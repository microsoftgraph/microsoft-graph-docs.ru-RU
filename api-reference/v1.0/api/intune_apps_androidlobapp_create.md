# <a name="create-androidlobapp"></a><span data-ttu-id="ae1a8-101">Создание androidLobApp</span><span class="sxs-lookup"><span data-stu-id="ae1a8-101">Create androidLobApp</span></span>

> <span data-ttu-id="ae1a8-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ae1a8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ae1a8-103">Создание нового объекта [androidLobApp](../resources/intune_apps_androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae1a8-103">Create a new [androidLobApp](../resources/intune_apps_androidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ae1a8-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="ae1a8-104">Prerequisites</span></span>
<span data-ttu-id="ae1a8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ae1a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ae1a8-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ae1a8-107">Permission type</span></span>|<span data-ttu-id="ae1a8-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ae1a8-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae1a8-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ae1a8-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ae1a8-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae1a8-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ae1a8-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ae1a8-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae1a8-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae1a8-112">Not supported.</span></span>|
|<span data-ttu-id="ae1a8-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ae1a8-113">Application</span></span>|<span data-ttu-id="ae1a8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae1a8-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae1a8-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ae1a8-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="ae1a8-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ae1a8-116">Request headers</span></span>
|<span data-ttu-id="ae1a8-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ae1a8-117">Header</span></span>|<span data-ttu-id="ae1a8-118">Значение</span><span class="sxs-lookup"><span data-stu-id="ae1a8-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae1a8-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ae1a8-119">Authorization</span></span>|<span data-ttu-id="ae1a8-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="ae1a8-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae1a8-121">Принять</span><span class="sxs-lookup"><span data-stu-id="ae1a8-121">Accept</span></span>|<span data-ttu-id="ae1a8-122">приложение/json</span><span class="sxs-lookup"><span data-stu-id="ae1a8-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae1a8-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ae1a8-123">Request body</span></span>
<span data-ttu-id="ae1a8-124">В теле запроса добавьте представление объекта androidLobApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ae1a8-124">In the request body, supply a JSON representation for the androidLobApp object.</span></span>

<span data-ttu-id="ae1a8-125">Ниже показаны свойства, которые необходимо указывать при создании объекта androidLobApp.</span><span class="sxs-lookup"><span data-stu-id="ae1a8-125">The following table shows the properties that are required when you create the androidLobApp.</span></span>

|<span data-ttu-id="ae1a8-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="ae1a8-126">Property</span></span>|<span data-ttu-id="ae1a8-127">Тип</span><span class="sxs-lookup"><span data-stu-id="ae1a8-127">Type</span></span>|<span data-ttu-id="ae1a8-128">Описание</span><span class="sxs-lookup"><span data-stu-id="ae1a8-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae1a8-129">id</span><span class="sxs-lookup"><span data-stu-id="ae1a8-129">id</span></span>|<span data-ttu-id="ae1a8-130">Строка</span><span class="sxs-lookup"><span data-stu-id="ae1a8-130">String</span></span>|<span data-ttu-id="ae1a8-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ae1a8-131">Key of the entity.</span></span> <span data-ttu-id="ae1a8-132">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae1a8-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ae1a8-133">displayName</span><span class="sxs-lookup"><span data-stu-id="ae1a8-133">displayName</span></span>|<span data-ttu-id="ae1a8-134">Строка</span><span class="sxs-lookup"><span data-stu-id="ae1a8-134">String</span></span>|<span data-ttu-id="ae1a8-135">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="ae1a8-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ae1a8-136">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae1a8-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ae1a8-137">описание</span><span class="sxs-lookup"><span data-stu-id="ae1a8-137">description</span></span>|<span data-ttu-id="ae1a8-138">Строка</span><span class="sxs-lookup"><span data-stu-id="ae1a8-138">String</span></span>|<span data-ttu-id="ae1a8-139">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="ae1a8-139">The description of the app.</span></span> <span data-ttu-id="ae1a8-140">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae1a8-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ae1a8-141">publisher</span><span class="sxs-lookup"><span data-stu-id="ae1a8-141">publisher</span></span>|<span data-ttu-id="ae1a8-142">Строка</span><span class="sxs-lookup"><span data-stu-id="ae1a8-142">String</span></span>|<span data-ttu-id="ae1a8-143">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="ae1a8-143">The publisher of the app.</span></span> <span data-ttu-id="ae1a8-144">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae1a8-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ae1a8-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ae1a8-145">largeIcon</span></span>|[<span data-ttu-id="ae1a8-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ae1a8-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="ae1a8-147">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="ae1a8-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ae1a8-148">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae1a8-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ae1a8-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ae1a8-149">createdDateTime</span></span>|<span data-ttu-id="ae1a8-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae1a8-150">DateTimeOffset</span></span>|<span data-ttu-id="ae1a8-151">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="ae1a8-151">The date and time the app was created.</span></span> <span data-ttu-id="ae1a8-152">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae1a8-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ae1a8-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ae1a8-153">lastModifiedDateTime</span></span>|<span data-ttu-id="ae1a8-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae1a8-154">DateTimeOffset</span></span>|<span data-ttu-id="ae1a8-155">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="ae1a8-155">The date and time the app was last modified.</span></span> <span data-ttu-id="ae1a8-156">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae1a8-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ae1a8-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ae1a8-157">isFeatured</span></span>|<span data-ttu-id="ae1a8-158">Логическое</span><span class="sxs-lookup"><span data-stu-id="ae1a8-158">Boolean</span></span>|<span data-ttu-id="ae1a8-159">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae1a8-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ae1a8-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ae1a8-160">privacyInformationUrl</span></span>|<span data-ttu-id="ae1a8-161">Строка</span><span class="sxs-lookup"><span data-stu-id="ae1a8-161">String</span></span>|<span data-ttu-id="ae1a8-162">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="ae1a8-162">The privacy statement Url.</span></span> <span data-ttu-id="ae1a8-163">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae1a8-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ae1a8-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ae1a8-164">informationUrl</span></span>|<span data-ttu-id="ae1a8-165">Строка</span><span class="sxs-lookup"><span data-stu-id="ae1a8-165">String</span></span>|<span data-ttu-id="ae1a8-166">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="ae1a8-166">The more information Url.</span></span> <span data-ttu-id="ae1a8-167">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae1a8-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ae1a8-168">owner</span><span class="sxs-lookup"><span data-stu-id="ae1a8-168">owner</span></span>|<span data-ttu-id="ae1a8-169">Строка</span><span class="sxs-lookup"><span data-stu-id="ae1a8-169">String</span></span>|<span data-ttu-id="ae1a8-170">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="ae1a8-170">The owner of the app.</span></span> <span data-ttu-id="ae1a8-171">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae1a8-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ae1a8-172">developer</span><span class="sxs-lookup"><span data-stu-id="ae1a8-172">developer</span></span>|<span data-ttu-id="ae1a8-173">Строка</span><span class="sxs-lookup"><span data-stu-id="ae1a8-173">String</span></span>|<span data-ttu-id="ae1a8-174">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="ae1a8-174">The developer of the app.</span></span> <span data-ttu-id="ae1a8-175">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae1a8-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ae1a8-176">notes</span><span class="sxs-lookup"><span data-stu-id="ae1a8-176">notes</span></span>|<span data-ttu-id="ae1a8-177">Строка</span><span class="sxs-lookup"><span data-stu-id="ae1a8-177">String</span></span>|<span data-ttu-id="ae1a8-178">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="ae1a8-178">Notes for the app.</span></span> <span data-ttu-id="ae1a8-179">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae1a8-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ae1a8-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="ae1a8-180">publishingState</span></span>|[<span data-ttu-id="ae1a8-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="ae1a8-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="ae1a8-182">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="ae1a8-182">The publishing state for the app.</span></span> <span data-ttu-id="ae1a8-183">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="ae1a8-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ae1a8-184">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae1a8-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span> <span data-ttu-id="ae1a8-185">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="ae1a8-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ae1a8-186">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="ae1a8-186">committedContentVersion</span></span>|<span data-ttu-id="ae1a8-187">Строка</span><span class="sxs-lookup"><span data-stu-id="ae1a8-187">String</span></span>|<span data-ttu-id="ae1a8-188">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="ae1a8-188">The internal committed content version.</span></span> <span data-ttu-id="ae1a8-189">Наследуется от объекта [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae1a8-189">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="ae1a8-190">fileName</span><span class="sxs-lookup"><span data-stu-id="ae1a8-190">fileName</span></span>|<span data-ttu-id="ae1a8-191">Строка</span><span class="sxs-lookup"><span data-stu-id="ae1a8-191">String</span></span>|<span data-ttu-id="ae1a8-192">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="ae1a8-192">The name of the main Lob application file.</span></span> <span data-ttu-id="ae1a8-193">Наследуется от объекта [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae1a8-193">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="ae1a8-194">size</span><span class="sxs-lookup"><span data-stu-id="ae1a8-194">size</span></span>|<span data-ttu-id="ae1a8-195">Int64</span><span class="sxs-lookup"><span data-stu-id="ae1a8-195">Int64</span></span>|<span data-ttu-id="ae1a8-196">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="ae1a8-196">The total size, including all uploaded files.</span></span> <span data-ttu-id="ae1a8-197">Наследуется от [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae1a8-197">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="ae1a8-198">packageId</span><span class="sxs-lookup"><span data-stu-id="ae1a8-198">packageId</span></span>|<span data-ttu-id="ae1a8-199">Строка</span><span class="sxs-lookup"><span data-stu-id="ae1a8-199">String</span></span>|<span data-ttu-id="ae1a8-200">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="ae1a8-200">The package identifier.</span></span>|
|<span data-ttu-id="ae1a8-201">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ae1a8-201">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="ae1a8-202">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ae1a8-202">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="ae1a8-203">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="ae1a8-203">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="ae1a8-204">versionName</span><span class="sxs-lookup"><span data-stu-id="ae1a8-204">versionName</span></span>|<span data-ttu-id="ae1a8-205">String (строка)</span><span class="sxs-lookup"><span data-stu-id="ae1a8-205">String</span></span>|<span data-ttu-id="ae1a8-206">Имя версии бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="ae1a8-206">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="ae1a8-207">versionCode</span><span class="sxs-lookup"><span data-stu-id="ae1a8-207">versionCode</span></span>|<span data-ttu-id="ae1a8-208">String (строка)</span><span class="sxs-lookup"><span data-stu-id="ae1a8-208">String</span></span>|<span data-ttu-id="ae1a8-209">Код версии бизнес-приложения Android.</span><span class="sxs-lookup"><span data-stu-id="ae1a8-209">The version code of Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="ae1a8-210">Ответ</span><span class="sxs-lookup"><span data-stu-id="ae1a8-210">Response</span></span>
<span data-ttu-id="ae1a8-211">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [androidLobApp](../resources/intune_apps_androidlobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ae1a8-211">If successful, this method returns a `201 Created` response code and a [androidLobApp](../resources/intune_apps_androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae1a8-212">Пример</span><span class="sxs-lookup"><span data-stu-id="ae1a8-212">Example</span></span>
### <a name="request"></a><span data-ttu-id="ae1a8-213">Запрос</span><span class="sxs-lookup"><span data-stu-id="ae1a8-213">Request</span></span>
<span data-ttu-id="ae1a8-214">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ae1a8-214">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1139

{
  "@odata.type": "#microsoft.graph.androidLobApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```

### <a name="response"></a><span data-ttu-id="ae1a8-215">Ответ</span><span class="sxs-lookup"><span data-stu-id="ae1a8-215">Response</span></span>
<span data-ttu-id="ae1a8-p118">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ae1a8-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1247

{
  "@odata.type": "#microsoft.graph.androidLobApp",
  "id": "4b9a27d0-27d0-4b9a-d027-9a4bd0279a4b",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```








