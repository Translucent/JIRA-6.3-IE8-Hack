<!--[if lt IE 9]>
<style type="text/css">
	body {
		overflow-y: scroll;
		-ms-overflow-y : scroll;
	}
</style>
<script>
	document.createElement('header');
	document.createElement('nav');
	document.createElement('section');
	document.createElement('article');
	document.createElement('aside');
	document.createElement('footer');
	document.createElement('hgroup');
</script>
<![endif]-->

<script type="text/javascript">

	function isIE () {
		var myNav = navigator.userAgent.toLowerCase();
		return (myNav.indexOf('msie') != -1) ? parseInt(myNav.split('msie')[1]) : false;
	}

	if(8 == isIE()) {

		// scrollbar is missing vhen viewing the issue browser
		setTimeout(function(){
			AJS.$("body").css("overflow-y", "scroll");
			AJS.$("body").css("-ms-overflow-y", "scroll");
		}, 1000);

		if(JIRA && JIRA.Components && JIRA.Components.IssueViewer && JIRA.Components.IssueViewer.Collections && JIRA.Components.IssueViewer.Collections.Panels) {

			// taken from 6.3.10 code
			JIRA.Components.IssueViewer.Collections.Panels.prototype.update = function (data, options) {
		        var instance = this;

		        this.each(function (panel) {
		        	if(panel != undefined) { // ie8: sometimes panel is undefined
			            var panelId = panel.id;
			            var panelPresentInPanelEntities = _.any(data, function (panel) {
			                return panel.id === panelId
			            });
			            if (!panelPresentInPanelEntities) {
			                this.remove(panel);
			            }
			        }
		        }, this);

		        _.each(data, function (entity, index) {
		            var panel = this.get(entity.id);
		            if (panel) {
		                panel.update(entity, options.fieldsInProgress, options.fieldsSaved);
		            } else {
		                this.add({id: entity.id, entity: entity}, {at: index});
		            }
		        }, this);
		    }
		}

		// define missing function forEach
		Array.prototype.forEach = function(callback, thisArg) {

		    var T, k;

		    if (this == null) {
		      throw new TypeError(' this is null or not defined');
		    }

		    var O = Object(this);

		    var len = O.length >>> 0;

		    if (typeof callback !== "function") {
		      throw new TypeError(callback + ' is not a function');
		    }

		    if (arguments.length > 1) {
		      T = thisArg;
		    }

		    k = 0;

		    while (k < len) {

		      var kValue;

		      if (k in O) {

		        kValue = O[k];

		        callback.call(T, kValue, k, O);
		      }
		      k++;
		    }
		  };

		// define missing function indexOf
		Array.prototype.indexOf = function(elt /*, from*/) {
		    var len = this.length >>> 0;

		    var from = Number(arguments[1]) || 0;
		    from = (from < 0)
		         ? Math.ceil(from)
		         : Math.floor(from);
		    if (from < 0)
		      from += len;

		    for (; from < len; from++)
		    {
		      if (from in this &&
		          this[from] === elt)
		        return from;
		    }
	    	return -1;
		};

		// Remove Activity Stream from project view page
		AJS.$(function(){
			AJS.$("div.activitystream-container").remove();
		});

		// remove Activity Stream gadget
		AJS.$(function(){
			if(typeof AG !== 'undefined' && AG.DashboardManager) {
				var addLayout_orig = AG.DashboardManager.addLayout; 
				var dbm = AG.DashboardManager;
				dbm.addLayout = function(descriptor) { 
					try {
						var dl = descriptor.gadgets;
						var nl = [];
						_.each(descriptor.gadgets, function(layout){
							if("Activity Stream" != layout.title) {
								nl.push(layout);
							}
						});
						descriptor.gadgets = nl;
					} catch(err){}
					addLayout_orig.apply(dbm, [descriptor]); 
				}
			}
		});
	}

</script>
