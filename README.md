
<main>
  <button> click me </button>
</main>

<script>
    const cssstr=`
    @import "https://unpkg.com/tofukit/tools/reset.css";
    main {     
      display: flex;
      justify-content: center;
      button {        
        font-size: 2em;
        padding: 1em 2em;
        border: none;
        border-radius: 5px;
        background-color: #0077cc;
        color: #fff;
        cursor: pointer;
        transition: background-color 0.3s ease;

        &:hover {          
          background-color: #005fa3;
          box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
          transform: scale(1.05);
        }
                
        &:active {         
          background-color: #003c66;
          box-shadow: 0 1px 2px rgba(0, 0, 0, 0.2);
          transform: scale(0.95);
        }      
      }
    }`

    const style = document.createElement('style');

    style.innerHTML = cssstr;

    document.head.appendChild(style);

</script>
