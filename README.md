import React from 'react';

interface MenuLinkProps {
  iconSrc: string;
  text: string;
  arrowSrc: string;
}

const MenuLink: React.FC<MenuLinkProps> = ({ iconSrc, text, arrowSrc }) => {
  return (
    <a href="#" className="flex overflow-hidden gap-2.5 items-center pt-2.5 pr-4 pb-3 pl-5 h-full rounded min-w-[240px]">
      <img loading="lazy" src={iconSrc} alt="" className="object-contain aspect-[0.67] w-[18px]" />
      <span className="self-stretch my-auto text-lg text-zinc-500">{text}</span>
      <img loading="lazy" src={arrowSrc} alt="" className="object-contain w-3 aspect-[0.67]" />
    </a>
  );
};

export default MenuLink;
