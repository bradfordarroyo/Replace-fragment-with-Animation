# Replace-fragment-with-Animation
Replace fragment with Animation
private void replaceFragment(Fragment fragment) {
    FragmentManager manager = getSupportFragmentManager();
   FragmentTransaction transaction = manager.beginTransaction();
   transaction.setCustomAnimations(R.anim.slide_in_right,R.anim.slide_out_left)
   .replace(R.id.content_main, fragment)
   .addToBackStack(null)
   .commit();
}
