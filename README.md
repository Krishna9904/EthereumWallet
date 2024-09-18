function App() {
  const [twoTrue, settwoTrue] = useState(false);
  return (
    <div className="grandfather">
      <div className="father">
        {twoTrue ? (
          <div className="main">
            <div className="grandson">
              <div>
                <input 
                  type="checkbox"
                  id="vehicle1"
                  name="vehicle1"
                  value={twoTrue}
                  onClick={() => settwoTrue(!twoTrue)}
                />
              </div>
              <div></div>
              <div>
                <input type="text"  className="inpu"/>
              </div>
            </div>
            <div className="son"></div>
          </div>
        ) : (
          <div className="grandson">
            <div>
              <input
                type="checkbox"
                id="vehicle1"
                name="vehicle1"
                value={twoTrue}
                onClick={() => settwoTrue(!twoTrue)}
              />
            </div>
            <div></div>
            <div>
              <input type="text"  className="inpu"/>
            </div>
          </div>
        )}
      </div>
    </div>
  );
}

export default App;


.main{
  display: grid;
  grid-template-columns:3fr 2fr;
  height: 100%;
}
.son{
  background-color: aqua;
}
.father{
  max-width: 70%;
  width: 100%;
  height: 95%;
  position: absolute;
  bottom:0px ;
  right: 0px;
  
}
.grandfather{
  position: relative;
  height: 100vh;
  
}
.grandson{
  display: flex;
  flex-direction: column;
  justify-content: space-between;
    height: 100%;
}
.inpu{
  margin-bottom: 100px;
}
