# WebDialog

>Step One : Add button to your document.

...<button id="btnShowDia">Show Dialog</button>...

>Step Two : Add css to button .

...#btnShowDia {
        padding: 15px;
        border: none;
        outline: none;
        border-radius: 10px;
        background-color: white;
        color: black;
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        cursor: pointer;
    }
...

>Step Three : Add Dialog in document.

... <dialog  id="popUpDia">
        <p class="tital"><b>Dialog</b> </p>
        <p class="desc">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ea, sequi repellat commodi numquam porro vel. Aliquam commodi distinctio eius? Possimus quae perferendis numquam hic dolor, commodi deleniti enim accusamus aspernatur.</p>
        <button id="btnCloseDia">Close</button>
    </dialog>...

>Strp Fore : Add CSS to dialog.

... #popUpDia {
        width: 300px;
        padding: 15px;
        border: none;
        outline: none;
        border-radius: 10px;
        background-color: white;
        color: black;
        position: absolute;
        cursor: pointer;
        text-align: center;
    }
  

    .tital {
        font-size: 30px;
        padding: 0;
        margin: 0;
    }
    .desc {
        color: gray;
    }

    #btnCloseDia {
        width: 100%;
        height: 45px;
        background-color: black;
        border-radius: 10px;
        color: white;
        cursor: pointer;
    }
...

>Step Five : Add JS to open and close dialog.

...
    const dialog = document.querySelector('#popUpDia');
    const showButton = document.querySelector('#btnShowDia');
    const CloseButton = document.querySelector('#btnCloseDia');

    showButton.addEventListener('click' , ()=>{
        dialog.showModal();

    })

    CloseButton.addEventListener('click' , ()=>{
        dialog.close();
    })...

![Screenshot (21)](https://user-images.githubusercontent.com/114288510/202205746-6939e0f4-a0d8-44af-a9be-3bc201cb453b.png)

![Screenshot (22)](https://user-images.githubusercontent.com/114288510/202205804-5bc8561f-065f-4b52-82db-e7413f860ea1.png)
