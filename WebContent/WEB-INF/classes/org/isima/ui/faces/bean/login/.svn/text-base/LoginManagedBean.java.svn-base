package org.isima.ui.faces.bean.login;

import javax.faces.application.FacesMessage;
import javax.faces.bean.ManagedBean;
import javax.faces.context.FacesContext;

@ManagedBean
public class LoginManagedBean {
	
	private String username ;
	private String password ;
	
	public String getUsername() {
		return username;
	}
	public void setUsername(String username) {
		this.username = username;
	}
	
	public String getPassword() {
		return password;
	}
	public void setPassword(String password) {
		this.password = password;
	}
	
	public String login(){
		//TODO
		if("admin".equals(username) && "admin".equals(password)){
			return "loginSuccess";
		}
		FacesContext.getCurrentInstance().addMessage(null, 
				new FacesMessage("Not authorized !"));
		return "loginFailed";
	}

}
