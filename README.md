<br />
<div class="container animated fadeIn">
    <hr />
    <h2 class='h2'>Install <a onclick="ga.push(['_trackEvent','Download','zip',this.href]);" href="{{data.project.download}}" class="btn btn-primary btn-lg pull-right">Download Zip</a></h2>
    <hr />
    <!--<div class="well row">-->
        <!--<div class="col-sm-12">-->
            <span><b>Download FrameBox from npm.</b></span>
            <pre><code class="TypeScript" pCode>npm install framebox@4.3.0 </code></pre>
        <!--</div>-->
        <!--<div class="col-sm-12">-->
            <span><b>Import FrameBoxModule from node_modules folder </b></span>
            <pre><code class="TypeScript" pCode>import &#123; FrameBoxModule &#125; from 'framebox';</code></pre>
        <!--</div>-->
        <!--<div class="col-sm-12">-->
            <span><b>Add FrameBoxModule to @ngModule imports. </b></span>
            <pre>
<code >
@NgModule(&#123;
    &nbsp;declarations: [
        &nbsp;&nbsp;AppComponent,
        &nbsp;&nbsp;NavbarComponent,
        &nbsp;&nbsp;FooterComponent
    &nbsp;],
    &nbsp;imports: [
        &nbsp;&nbsp;BrowserModule,
        &nbsp;&nbsp;FormsModule,
        &nbsp;&nbsp;HttpModule,
        &nbsp;&nbsp;<b>FrameBoxModule</b>
    &nbsp;],
    &nbsp;providers: [DataService],
    &nbsp;bootstrap: [AppComponent]
&#125;)   
                </code>
</pre>
        <!--</div>-->

    <!--</div>-->
    <hr />
    <h2>Usage</h2>
    <hr />  
            <p class="lead">Typical Angular 2 component using typescript.</p>
            <p></p>
            <pre><code >
import &#123; Component &#125; from &#x27;@angular/core&#x27;;
@Component(&#123;
    selector: &#x27;home&#x27;,
    templateUrl: &#x27;./home.component.html&#x27;
&#125;)
export class HomeComponent &#123;
    pieceName: string = &#x22;Dog Heaven 4&#x22;;
    selectedPieceName: string = &#x22;&#x22;;
    imageLocation: string = &#x22;&#x22;;
    image: string = &#x22;http://wylandflorida.com/Images/JimWarren/65/thumbsXL/thumb_Dog Heaven 4.jpg&#x22;;
    frameStyle: string = &#x22;Package_2552&#x22;;

    constructor() &#123; &#125;

&#125;         
                </code></pre>

            <p class="lead">Typical Template using Twitter Bootstrap</p>
            <pre><code class="html" pCode>
&#x3C;div class=&#x22;row&#x22;&#x3E;
    &#x3C;div class=&#x22;well col-lg-8 col-md-9 col-sm-12 col-xs-12&#x22;&#x3E;
        &#x3C;framebox [image]=&#x22;image&#x22; [pieceName]=&#x22;pieceName&#x22; [frameStyle]=&#x22;frameStyle&#x22; [EnableSelection]=&#x22;false&#x22;&#x3E;&#x3C;/framebox&#x3E;
        &#x3C;/div&#x3E;
    &#x3C;div class=&#x22;well col-lg-4 col-md-3 col-sm-12 col-xs-12&#x22;&#x3E;
        &#x3C;framebox-selection [(frameStyle)]=&#x22;frameStyle&#x22;&#x3E;&#x3C;/framebox-selection&#x3E;
    &#x3C;/div&#x3E;
&#x3C;/div&#x3E;                
                </code></pre>


    <h2>Selectors</h2>
    <hr />

 
            <b class="lead">[framebox]:</b>
            <pre><code class="TypeScript" pCode><b class="lead">&#x3C;framebox&#x3E;&#x3C;/ framebox&#x3E;</b></code></pre>

            <span><b class="lead">Attributes:</b></span>
            <table class="table table-responsive table-bordered table-hover">
                <thead style="background-color:white;color:black;">
                    <tr>
                        <th>Name</th>
                        <th>Type</th>
                        <th>Description</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>[image]</td>
                        <td>(string)</td>
                        <td>Your image URL.</td>
                    </tr>
                    <tr>
                        <td>[pieceName]</td>
                        <td>(string)</td>
                        <td>Name of Image.</td>
                    </tr>
                    <tr>
                        <td>[EnableSelection]</td>
                        <td>(boolean)</td>
                        <td>Enables or disables frame selection on hover.</td>
                    </tr>
                    <tr>
                        <td>[frameStyle]</td>
                        <td>(string)</td>
                        <td>
                            List of available packages:<br />
                            <i style="color:yellow">
                                Package_2514,
                                Package_2515,
                                Package_2516,
                                Package_2517,
                                Package_2519,
                                Package_2525,
                                Package_2544,
                                Package_2533,
                                Package_2552,
                                Package_2554,
                                Package_2559,
                                Package_2566,
                                Package_2567,
                                Package_2569,
                                Package_2571
                            </i>
                        </td>
                    </tr>

                </tbody>
            </table>

            <hr />

            <b class="lead">[framebox-selection]:</b>
            <pre><code class="html" pCode>&lt;framebox-selection [(frameStyle)]="frameStyle"&gt;&lt;/framebox-selection&gt;</code></pre>
            <table class="table table-responsive table-bordered table-hover">
                <thead style="background-color:white;color:black;">
                    <tr>
                        <th>Name</th>
                        <th>Type</th>
                        <th>Description</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>[frameStyle]</td>
                        <td>(string)</td>
                        <td>
                            List of available packages:<br />

                            <i style="color:yellow">
                                Package_2514,
                                Package_2515,
                                Package_2516,
                                Package_2517,
                                Package_2519,
                                Package_2525,
                                Package_2544,
                                Package_2533,
                                Package_2552,
                                Package_2554,
                                Package_2559,
                                Package_2566,
                                Package_2567,
                                Package_2569,
                                Package_2571
                            </i>
                        </td>
                    </tr>
                </tbody>
            </table>


</div>
