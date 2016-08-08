# wanme
owner
@Override
    public View onCreateView(LayoutInflater inflater, ViewGroup container, Bundle savedInstanceState) {
        View view = inflater.inflate(R.layout.fragment_find, container, false);
        mSlideImageView = (SlideImageView) view.findViewById(R.id.slide_imageview);
        imageView = (ImageView) view.findViewById(R.id.imageView);

        ImageCacheManger.loadImage(URL, imageView,
                getBitmapFromResources(getActivity(), R.drawable.ic_launcher), getBitmapFromResources(getActivity(), R.drawable.error));
        imageView.setOnClickListener(this);
