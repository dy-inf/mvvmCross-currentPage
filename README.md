    public class MainViewModel : MvxViewModel
    {
        private Page _customPage = new CustomPage();
    
        private Page _activePage;
        public Page ActivePage
        {
            get => _activePage;
            set => SetProperty(ref _activePage, value);
        }
    
        public MainViewModel() 
        {
            ActivePage = _customPage;
        }
    }
