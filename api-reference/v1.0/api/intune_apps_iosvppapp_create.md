# <a name="create-iosvppapp"></a><span data-ttu-id="73897-101">Создание iosVppApp</span><span class="sxs-lookup"><span data-stu-id="73897-101">Create iosVppApp</span></span>

> <span data-ttu-id="73897-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="73897-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="73897-103">Создание объекта [iosVppApp](../resources/intune_apps_iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="73897-103">Create a new [iosVppApp](../resources/intune_apps_iosvppapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="73897-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="73897-104">Prerequisites</span></span>
<span data-ttu-id="73897-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="73897-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="73897-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="73897-107">Permission type</span></span>|<span data-ttu-id="73897-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="73897-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73897-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73897-109">Delegated (work or school account)</span></span>|<span data-ttu-id="73897-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73897-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="73897-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73897-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73897-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73897-112">Not supported.</span></span>|
|<span data-ttu-id="73897-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="73897-113">Application</span></span>|<span data-ttu-id="73897-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73897-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="73897-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73897-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="73897-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="73897-116">Request headers</span></span>
|<span data-ttu-id="73897-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="73897-117">Header</span></span>|<span data-ttu-id="73897-118">Значение</span><span class="sxs-lookup"><span data-stu-id="73897-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73897-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="73897-119">Authorization</span></span>|<span data-ttu-id="73897-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="73897-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73897-121">Accept</span><span class="sxs-lookup"><span data-stu-id="73897-121">Accept</span></span>|<span data-ttu-id="73897-122">application/json</span><span class="sxs-lookup"><span data-stu-id="73897-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73897-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="73897-123">Request body</span></span>
<span data-ttu-id="73897-124">В тексте запроса добавьте представление объекта iosVppApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="73897-124">In the request body, supply a JSON representation for the iosVppApp object.</span></span>

<span data-ttu-id="73897-125">В приведенной ниже таблице показаны, которые необходимо указывать при создании объекта iosVppApp.</span><span class="sxs-lookup"><span data-stu-id="73897-125">The following table shows the properties that are required when you create the iosVppApp.</span></span>

|<span data-ttu-id="73897-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="73897-126">Property</span></span>|<span data-ttu-id="73897-127">Тип</span><span class="sxs-lookup"><span data-stu-id="73897-127">Type</span></span>|<span data-ttu-id="73897-128">Описание</span><span class="sxs-lookup"><span data-stu-id="73897-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73897-129">id</span><span class="sxs-lookup"><span data-stu-id="73897-129">id</span></span>|<span data-ttu-id="73897-130">Строка</span><span class="sxs-lookup"><span data-stu-id="73897-130">String</span></span>|<span data-ttu-id="73897-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="73897-131">Key of the entity.</span></span> <span data-ttu-id="73897-132">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73897-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73897-133">displayName</span><span class="sxs-lookup"><span data-stu-id="73897-133">displayName</span></span>|<span data-ttu-id="73897-134">String (строка)</span><span class="sxs-lookup"><span data-stu-id="73897-134">String</span></span>|<span data-ttu-id="73897-135">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="73897-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="73897-136">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73897-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73897-137">description</span><span class="sxs-lookup"><span data-stu-id="73897-137">description</span></span>|<span data-ttu-id="73897-138">String (строка)</span><span class="sxs-lookup"><span data-stu-id="73897-138">String</span></span>|<span data-ttu-id="73897-139">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="73897-139">The description of the app.</span></span> <span data-ttu-id="73897-140">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73897-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73897-141">publisher</span><span class="sxs-lookup"><span data-stu-id="73897-141">publisher</span></span>|<span data-ttu-id="73897-142">String (строка)</span><span class="sxs-lookup"><span data-stu-id="73897-142">String</span></span>|<span data-ttu-id="73897-143">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="73897-143">The publisher of the app.</span></span> <span data-ttu-id="73897-144">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73897-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73897-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="73897-145">largeIcon</span></span>|[<span data-ttu-id="73897-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="73897-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="73897-147">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="73897-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="73897-148">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73897-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73897-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="73897-149">createdDateTime</span></span>|<span data-ttu-id="73897-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73897-150">DateTimeOffset</span></span>|<span data-ttu-id="73897-151">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="73897-151">The date and time the app was created.</span></span> <span data-ttu-id="73897-152">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73897-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73897-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="73897-153">lastModifiedDateTime</span></span>|<span data-ttu-id="73897-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73897-154">DateTimeOffset</span></span>|<span data-ttu-id="73897-155">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="73897-155">The date and time the app was last modified.</span></span> <span data-ttu-id="73897-156">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73897-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73897-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="73897-157">isFeatured</span></span>|<span data-ttu-id="73897-158">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="73897-158">Boolean</span></span>|<span data-ttu-id="73897-159">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73897-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73897-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="73897-160">privacyInformationUrl</span></span>|<span data-ttu-id="73897-161">String (строка)</span><span class="sxs-lookup"><span data-stu-id="73897-161">String</span></span>|<span data-ttu-id="73897-162">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="73897-162">The privacy statement Url.</span></span> <span data-ttu-id="73897-163">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73897-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73897-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="73897-164">informationUrl</span></span>|<span data-ttu-id="73897-165">String (строка)</span><span class="sxs-lookup"><span data-stu-id="73897-165">String</span></span>|<span data-ttu-id="73897-166">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="73897-166">The more information Url.</span></span> <span data-ttu-id="73897-167">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73897-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73897-168">owner</span><span class="sxs-lookup"><span data-stu-id="73897-168">owner</span></span>|<span data-ttu-id="73897-169">String (строка)</span><span class="sxs-lookup"><span data-stu-id="73897-169">String</span></span>|<span data-ttu-id="73897-170">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="73897-170">The owner of the app.</span></span> <span data-ttu-id="73897-171">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73897-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73897-172">developer</span><span class="sxs-lookup"><span data-stu-id="73897-172">developer</span></span>|<span data-ttu-id="73897-173">String (строка)</span><span class="sxs-lookup"><span data-stu-id="73897-173">String</span></span>|<span data-ttu-id="73897-174">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="73897-174">The developer of the app.</span></span> <span data-ttu-id="73897-175">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73897-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73897-176">notes</span><span class="sxs-lookup"><span data-stu-id="73897-176">notes</span></span>|<span data-ttu-id="73897-177">String (строка)</span><span class="sxs-lookup"><span data-stu-id="73897-177">String</span></span>|<span data-ttu-id="73897-178">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="73897-178">Notes for the app.</span></span> <span data-ttu-id="73897-179">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73897-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73897-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="73897-180">publishingState</span></span>|[<span data-ttu-id="73897-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="73897-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="73897-182">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="73897-182">The publishing state for the app.</span></span> <span data-ttu-id="73897-183">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="73897-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="73897-184">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73897-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span> <span data-ttu-id="73897-185">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="73897-185">The possible values are `notPublished`, `processing`, `published`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="73897-186">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="73897-186">usedLicenseCount</span></span>|<span data-ttu-id="73897-187">Int32</span><span class="sxs-lookup"><span data-stu-id="73897-187">Int32</span></span>|<span data-ttu-id="73897-188">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="73897-188">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="73897-189">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="73897-189">totalLicenseCount</span></span>|<span data-ttu-id="73897-190">Int32</span><span class="sxs-lookup"><span data-stu-id="73897-190">Int32</span></span>|<span data-ttu-id="73897-191">Общее количество лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="73897-191">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="73897-192">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="73897-192">releaseDateTime</span></span>|<span data-ttu-id="73897-193">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73897-193">DateTimeOffset</span></span>|<span data-ttu-id="73897-194">Дата и время выпуска приложения, на которое распространяется программа VPP.</span><span class="sxs-lookup"><span data-stu-id="73897-194">The VPP application release date and time.</span></span>|
|<span data-ttu-id="73897-195">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="73897-195">appStoreUrl</span></span>|<span data-ttu-id="73897-196">String (строка)</span><span class="sxs-lookup"><span data-stu-id="73897-196">String</span></span>|<span data-ttu-id="73897-197">URL-адрес магазина.</span><span class="sxs-lookup"><span data-stu-id="73897-197">The store URL.</span></span>|
|<span data-ttu-id="73897-198">licensingType</span><span class="sxs-lookup"><span data-stu-id="73897-198">licensingType</span></span>|[<span data-ttu-id="73897-199">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="73897-199">vppLicensingType</span></span>](../resources/intune_apps_vpplicensingtype.md)|<span data-ttu-id="73897-200">Поддерживаемый тип лицензии.</span><span class="sxs-lookup"><span data-stu-id="73897-200">The supported License Type.</span></span>|
|<span data-ttu-id="73897-201">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="73897-201">applicableDeviceType</span></span>|[<span data-ttu-id="73897-202">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="73897-202">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="73897-203">Применимый тип устройства с iOS.</span><span class="sxs-lookup"><span data-stu-id="73897-203">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="73897-204">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="73897-204">vppTokenOrganizationName</span></span>|<span data-ttu-id="73897-205">String (строка)</span><span class="sxs-lookup"><span data-stu-id="73897-205">String</span></span>|<span data-ttu-id="73897-206">Организация, связанная с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="73897-206">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="73897-207">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="73897-207">vppTokenAccountType</span></span>|[<span data-ttu-id="73897-208">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="73897-208">vppTokenAccountType</span></span>](../resources/intune_shared_vpptokenaccounttype.md)|<span data-ttu-id="73897-209">Тип программы оптовых покупок, с которой связан заданный маркер Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="73897-209">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="73897-210">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="73897-210">The possible values are:</span></span> <span data-ttu-id="73897-211">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="73897-211">The possible values are:</span></span>|
|<span data-ttu-id="73897-212">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="73897-212">vppTokenAppleId</span></span>|<span data-ttu-id="73897-213">String (строка)</span><span class="sxs-lookup"><span data-stu-id="73897-213">String</span></span>|<span data-ttu-id="73897-214">Идентификатор Apple ID, связанный с заданным токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="73897-214">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="73897-215">bundleId</span><span class="sxs-lookup"><span data-stu-id="73897-215">bundleId</span></span>|<span data-ttu-id="73897-216">String (строка)</span><span class="sxs-lookup"><span data-stu-id="73897-216">String</span></span>|<span data-ttu-id="73897-217">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="73897-217">The Identity Name.</span></span>|



## <a name="response"></a><span data-ttu-id="73897-218">Ответ</span><span class="sxs-lookup"><span data-stu-id="73897-218">Response</span></span>
<span data-ttu-id="73897-219">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosVppApp](../resources/intune_apps_iosvppapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="73897-219">If successful, this method returns a `201 Created` response code and a [iosVppApp](../resources/intune_apps_iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73897-220">Пример</span><span class="sxs-lookup"><span data-stu-id="73897-220">Example</span></span>
### <a name="request"></a><span data-ttu-id="73897-221">Запрос</span><span class="sxs-lookup"><span data-stu-id="73897-221">Request</span></span>
<span data-ttu-id="73897-222">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="73897-222">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1286

{
  "@odata.type": "#microsoft.graph.iosVppApp",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value"
}
```

### <a name="response"></a><span data-ttu-id="73897-223">Ответ</span><span class="sxs-lookup"><span data-stu-id="73897-223">Response</span></span>
<span data-ttu-id="73897-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="73897-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1394

{
  "@odata.type": "#microsoft.graph.iosVppApp",
  "id": "a0ac9b6f-9b6f-a0ac-6f9b-aca06f9baca0",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value"
}
```



