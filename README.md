```mermaid
graph TD
    %% Phase 1: Initialization & Loading
    Start([Form Constructed<br/>compPid + yycode passed in]) --> Load[reportmenu_Load<br/>Triggered on form open]
    
    subgraph Form Initialization
        Load --> Clear[ClearControlsAndResetInputs<br/>Clears TextBoxes & UI inputs]
        Clear --> LoadData[LoadDataFromSQL<br/>Query sabreptopleft WHERE pid=pid]
        
    %% ... (the rest of the code goes here) ...

    class ComboChange,Keys,CloseForm,F3Debug,SQLLog,Reload,MKSEdit action;
