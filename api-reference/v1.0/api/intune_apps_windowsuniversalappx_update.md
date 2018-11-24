# <a name="update-windowsuniversalappx"></a><span data-ttu-id="ffdaa-101">Update windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="ffdaa-101">Update windowsUniversalAppX</span></span>

> <span data-ttu-id="ffdaa-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ffdaa-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ffdaa-103">Обновление свойств объекта [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="ffdaa-103">Update the properties of a [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ffdaa-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="ffdaa-104">Prerequisites</span></span>
<span data-ttu-id="ffdaa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ffdaa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ffdaa-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ffdaa-107">Permission type</span></span>|<span data-ttu-id="ffdaa-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ffdaa-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ffdaa-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ffdaa-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ffdaa-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffdaa-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ffdaa-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ffdaa-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ffdaa-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffdaa-112">Not supported.</span></span>|
|<span data-ttu-id="ffdaa-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ffdaa-113">Application</span></span>|<span data-ttu-id="ffdaa-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffdaa-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ffdaa-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ffdaa-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="ffdaa-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ffdaa-116">Request headers</span></span>
|<span data-ttu-id="ffdaa-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ffdaa-117">Header</span></span>|<span data-ttu-id="ffdaa-118">Значение</span><span class="sxs-lookup"><span data-stu-id="ffdaa-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ffdaa-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="ffdaa-119">Authorization</span></span>|<span data-ttu-id="ffdaa-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ffdaa-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ffdaa-121">Accept</span><span class="sxs-lookup"><span data-stu-id="ffdaa-121">Accept</span></span>|<span data-ttu-id="ffdaa-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ffdaa-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ffdaa-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ffdaa-123">Request body</span></span>
<span data-ttu-id="ffdaa-124">В теле запроса добавьте представление объекта [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ffdaa-124">In the request body, supply a JSON representation for the [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) object.</span></span>

<span data-ttu-id="ffdaa-125">Ниже показаны свойства, которые необходимо указывать при создании объекта [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="ffdaa-125">The following table shows the properties that are required when you create the [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md).</span></span>

|<span data-ttu-id="ffdaa-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="ffdaa-126">Property</span></span>|<span data-ttu-id="ffdaa-127">Тип</span><span class="sxs-lookup"><span data-stu-id="ffdaa-127">Type</span></span>|<span data-ttu-id="ffdaa-128">Описание</span><span class="sxs-lookup"><span data-stu-id="ffdaa-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffdaa-129">id</span><span class="sxs-lookup"><span data-stu-id="ffdaa-129">id</span></span>|<span data-ttu-id="ffdaa-130">String</span><span class="sxs-lookup"><span data-stu-id="ffdaa-130">String</span></span>|<span data-ttu-id="ffdaa-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ffdaa-131">Key of the entity.</span></span> <span data-ttu-id="ffdaa-132">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ffdaa-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ffdaa-133">displayName</span><span class="sxs-lookup"><span data-stu-id="ffdaa-133">displayName</span></span>|<span data-ttu-id="ffdaa-134">String</span><span class="sxs-lookup"><span data-stu-id="ffdaa-134">String</span></span>|<span data-ttu-id="ffdaa-135">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="ffdaa-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ffdaa-136">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ffdaa-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ffdaa-137">description</span><span class="sxs-lookup"><span data-stu-id="ffdaa-137">description</span></span>|<span data-ttu-id="ffdaa-138">String</span><span class="sxs-lookup"><span data-stu-id="ffdaa-138">String</span></span>|<span data-ttu-id="ffdaa-139">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="ffdaa-139">The description of the app.</span></span> <span data-ttu-id="ffdaa-140">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ffdaa-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ffdaa-141">publisher</span><span class="sxs-lookup"><span data-stu-id="ffdaa-141">publisher</span></span>|<span data-ttu-id="ffdaa-142">String</span><span class="sxs-lookup"><span data-stu-id="ffdaa-142">String</span></span>|<span data-ttu-id="ffdaa-143">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="ffdaa-143">The publisher of the app.</span></span> <span data-ttu-id="ffdaa-144">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ffdaa-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ffdaa-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ffdaa-145">largeIcon</span></span>|[<span data-ttu-id="ffdaa-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ffdaa-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="ffdaa-147">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="ffdaa-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ffdaa-148">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ffdaa-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ffdaa-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ffdaa-149">createdDateTime</span></span>|<span data-ttu-id="ffdaa-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ffdaa-150">DateTimeOffset</span></span>|<span data-ttu-id="ffdaa-151">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="ffdaa-151">The date and time the app was created.</span></span> <span data-ttu-id="ffdaa-152">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ffdaa-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ffdaa-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ffdaa-153">lastModifiedDateTime</span></span>|<span data-ttu-id="ffdaa-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ffdaa-154">DateTimeOffset</span></span>|<span data-ttu-id="ffdaa-155">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="ffdaa-155">The date and time the app was last modified.</span></span> <span data-ttu-id="ffdaa-156">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ffdaa-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ffdaa-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ffdaa-157">isFeatured</span></span>|<span data-ttu-id="ffdaa-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffdaa-158">Boolean</span></span>|<span data-ttu-id="ffdaa-159">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ffdaa-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ffdaa-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ffdaa-160">privacyInformationUrl</span></span>|<span data-ttu-id="ffdaa-161">String</span><span class="sxs-lookup"><span data-stu-id="ffdaa-161">String</span></span>|<span data-ttu-id="ffdaa-162">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="ffdaa-162">The privacy statement Url.</span></span> <span data-ttu-id="ffdaa-163">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ffdaa-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ffdaa-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ffdaa-164">informationUrl</span></span>|<span data-ttu-id="ffdaa-165">String</span><span class="sxs-lookup"><span data-stu-id="ffdaa-165">String</span></span>|<span data-ttu-id="ffdaa-166">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="ffdaa-166">The more information Url.</span></span> <span data-ttu-id="ffdaa-167">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ffdaa-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ffdaa-168">owner</span><span class="sxs-lookup"><span data-stu-id="ffdaa-168">owner</span></span>|<span data-ttu-id="ffdaa-169">String</span><span class="sxs-lookup"><span data-stu-id="ffdaa-169">String</span></span>|<span data-ttu-id="ffdaa-170">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="ffdaa-170">The owner of the app.</span></span> <span data-ttu-id="ffdaa-171">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ffdaa-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ffdaa-172">developer</span><span class="sxs-lookup"><span data-stu-id="ffdaa-172">developer</span></span>|<span data-ttu-id="ffdaa-173">String</span><span class="sxs-lookup"><span data-stu-id="ffdaa-173">String</span></span>|<span data-ttu-id="ffdaa-174">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="ffdaa-174">The developer of the app.</span></span> <span data-ttu-id="ffdaa-175">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ffdaa-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ffdaa-176">notes</span><span class="sxs-lookup"><span data-stu-id="ffdaa-176">notes</span></span>|<span data-ttu-id="ffdaa-177">String</span><span class="sxs-lookup"><span data-stu-id="ffdaa-177">String</span></span>|<span data-ttu-id="ffdaa-178">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="ffdaa-178">Notes for the app.</span></span> <span data-ttu-id="ffdaa-179">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ffdaa-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ffdaa-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="ffdaa-180">publishingState</span></span>|[<span data-ttu-id="ffdaa-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="ffdaa-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="ffdaa-182">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="ffdaa-182">The publishing state for the app.</span></span> <span data-ttu-id="ffdaa-183">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="ffdaa-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ffdaa-184">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ffdaa-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md).</span></span> <span data-ttu-id="ffdaa-185">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="ffdaa-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ffdaa-186">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="ffdaa-186">committedContentVersion</span></span>|<span data-ttu-id="ffdaa-187">String</span><span class="sxs-lookup"><span data-stu-id="ffdaa-187">String</span></span>|<span data-ttu-id="ffdaa-188">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="ffdaa-188">The internal committed content version.</span></span> <span data-ttu-id="ffdaa-189">Наследуется от объекта [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ffdaa-189">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="ffdaa-190">fileName</span><span class="sxs-lookup"><span data-stu-id="ffdaa-190">fileName</span></span>|<span data-ttu-id="ffdaa-191">String</span><span class="sxs-lookup"><span data-stu-id="ffdaa-191">String</span></span>|<span data-ttu-id="ffdaa-192">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="ffdaa-192">The name of the main Lob application file.</span></span> <span data-ttu-id="ffdaa-193">Наследуется от объекта [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ffdaa-193">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="ffdaa-194">size</span><span class="sxs-lookup"><span data-stu-id="ffdaa-194">size</span></span>|<span data-ttu-id="ffdaa-195">Int64</span><span class="sxs-lookup"><span data-stu-id="ffdaa-195">Int64</span></span>|<span data-ttu-id="ffdaa-196">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="ffdaa-196">The total size, including all uploaded files.</span></span> <span data-ttu-id="ffdaa-197">Наследуется от объекта [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ffdaa-197">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="ffdaa-198">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="ffdaa-198">applicableArchitectures</span></span>|[<span data-ttu-id="ffdaa-199">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="ffdaa-199">windowsArchitecture</span></span>](../resources/intune_apps_windowsarchitecture.md)|<span data-ttu-id="ffdaa-200">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="ffdaa-200">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="ffdaa-201">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="ffdaa-201">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="ffdaa-202">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="ffdaa-202">applicableDeviceTypes</span></span>|[<span data-ttu-id="ffdaa-203">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="ffdaa-203">windowsDeviceType</span></span>](../resources/intune_apps_windowsdevicetype.md)|<span data-ttu-id="ffdaa-204">Типы устройств с Windows, которые поддерживаются этим приложением.</span><span class="sxs-lookup"><span data-stu-id="ffdaa-204">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="ffdaa-205">Возможные значения: `none`, `desktop`, `mobile`, `holographic`, `team`.</span><span class="sxs-lookup"><span data-stu-id="ffdaa-205">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="ffdaa-206">identityName</span><span class="sxs-lookup"><span data-stu-id="ffdaa-206">identityName</span></span>|<span data-ttu-id="ffdaa-207">String</span><span class="sxs-lookup"><span data-stu-id="ffdaa-207">String</span></span>|<span data-ttu-id="ffdaa-208">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="ffdaa-208">The Identity Name.</span></span>|
|<span data-ttu-id="ffdaa-209">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="ffdaa-209">identityPublisherHash</span></span>|<span data-ttu-id="ffdaa-210">String</span><span class="sxs-lookup"><span data-stu-id="ffdaa-210">String</span></span>|<span data-ttu-id="ffdaa-211">Хэш издателей удостоверений.</span><span class="sxs-lookup"><span data-stu-id="ffdaa-211">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="ffdaa-212">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="ffdaa-212">identityResourceIdentifier</span></span>|<span data-ttu-id="ffdaa-213">String</span><span class="sxs-lookup"><span data-stu-id="ffdaa-213">String</span></span>|<span data-ttu-id="ffdaa-214">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="ffdaa-214">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="ffdaa-215">isBundle</span><span class="sxs-lookup"><span data-stu-id="ffdaa-215">isBundle</span></span>|<span data-ttu-id="ffdaa-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffdaa-216">Boolean</span></span>|<span data-ttu-id="ffdaa-217">Указывает, является ли приложение пакетом.</span><span class="sxs-lookup"><span data-stu-id="ffdaa-217">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="ffdaa-218">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ffdaa-218">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="ffdaa-219">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ffdaa-219">windowsMinimumOperatingSystem</span></span>](../resources/intune_apps_windowsminimumoperatingsystem.md)|<span data-ttu-id="ffdaa-220">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="ffdaa-220">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="ffdaa-221">identityVersion</span><span class="sxs-lookup"><span data-stu-id="ffdaa-221">identityVersion</span></span>|<span data-ttu-id="ffdaa-222">String</span><span class="sxs-lookup"><span data-stu-id="ffdaa-222">String</span></span>|<span data-ttu-id="ffdaa-223">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="ffdaa-223">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="ffdaa-224">Ответ</span><span class="sxs-lookup"><span data-stu-id="ffdaa-224">Response</span></span>
<span data-ttu-id="ffdaa-225">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ffdaa-225">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ffdaa-226">Пример</span><span class="sxs-lookup"><span data-stu-id="ffdaa-226">Example</span></span>
### <a name="request"></a><span data-ttu-id="ffdaa-227">Запрос</span><span class="sxs-lookup"><span data-stu-id="ffdaa-227">Request</span></span>
<span data-ttu-id="ffdaa-228">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ffdaa-228">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1189

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
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
  "applicableArchitectures": "x86",
  "applicableDeviceTypes": "desktop",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true
  },
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="ffdaa-229">Ответ</span><span class="sxs-lookup"><span data-stu-id="ffdaa-229">Response</span></span>
<span data-ttu-id="ffdaa-p120">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="ffdaa-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1361

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
  "id": "4bc47eba-7eba-4bc4-ba7e-c44bba7ec44b",
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
  "applicableArchitectures": "x86",
  "applicableDeviceTypes": "desktop",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true
  },
  "identityVersion": "Identity Version value"
}
```



