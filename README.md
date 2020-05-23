In order to add a custom banner you need to create a github account and create a branch from this repository.

Add the banner data to the end of the sql file you choose (global or jp or both) and open up a pull request.

Once I approve the pull request, the banner will immediately be added to the plazmid summon simulator.

Banner Data must be formatted as follows:

Global:

INSERT INTO plazmid_sim_banners_glb(id,banner_id,name,type,year,image,featured_r_rate,unfeatured_r_rate,unfeatured_r_count,featured_r_count,featured_sr_rate,unfeatured_sr_rate,unfeatured_sr_count,featured_sr_count,featured_ssr_rate,unfeatured_ssr_rate,unfeatured_ssr_count,featured_ssr_count,unfeatured,featured,unfeatured_gssr_rate,featured_gssr_rate,enabled)
VALUES(id (must be over 10000 and not aready exist),banner_id (must not already exist),"banner name in quotes",5,current_year,"banner_image_url(in quotes)",0.0(featured r rate),30.0(unfeatured r rate),0(total unfeatured rs),0(total featured rs),35.0(featured sr rate),25.0(unfeatured sr rate),0(total unfeatured srs),0(total featured srs),5.0(featured ssr rate),5.0(unfeatured ssr rate),0(total unfeatured ssrs),0(total featured ssrs),"1003972,1003971"(unfeatured cards),"1003970"(featured cards),95.0(unfeatured gssr rate),5.0(featured gssr rate),1);

JP:

INSERT INTO plazmid_sim_banners_jp(id,banner_id,name,type,year,image,featured_r_rate,unfeatured_r_rate,unfeatured_r_count,featured_r_count,featured_sr_rate,unfeatured_sr_rate,unfeatured_sr_count,featured_sr_count,featured_ssr_rate,unfeatured_ssr_rate,unfeatured_ssr_count,featured_ssr_count,unfeatured,featured,unfeatured_gssr_rate,featured_gssr_rate,enabled)
VALUES(id (must be over 10000 and not aready exist),banner_id (must not already exist),"banner name in quotes",5,current_year,"banner_image_url(in quotes)",0.0(featured r rate),30.0(unfeatured r rate),0(total unfeatured rs),0(total featured rs),35.0(featured sr rate),25.0(unfeatured sr rate),0(total unfeatured srs),0(total featured srs),5.0(featured ssr rate),5.0(unfeatured ssr rate),0(total unfeatured ssrs),0(total featured ssrs),"1003972,1003971"(unfeatured cards),"1003970"(featured cards),95.0(unfeatured gssr rate),5.0(featured gssr rate),1);
