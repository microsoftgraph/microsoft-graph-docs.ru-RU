# <a name="update-windowsuniversalappx"></a><span data-ttu-id="ddd4a-101">Update windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="ddd4a-101">Update windowsUniversalAppX</span></span>

> <span data-ttu-id="ddd4a-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ddd4a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ddd4a-103">Обновление свойств объекта [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="ddd4a-103">Update the properties of a [calendar](../resources/intune_apps_windowsuniversalappx.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ddd4a-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="ddd4a-104">Prerequisites</span></span>
<span data-ttu-id="ddd4a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ddd4a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ddd4a-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ddd4a-107">Permission type</span></span>|<span data-ttu-id="ddd4a-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ddd4a-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ddd4a-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ddd4a-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ddd4a-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddd4a-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ddd4a-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ddd4a-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ddd4a-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddd4a-112">Not supported.</span></span>|
|<span data-ttu-id="ddd4a-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ddd4a-113">Application</span></span>|<span data-ttu-id="ddd4a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddd4a-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ddd4a-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ddd4a-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="ddd4a-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ddd4a-116">Request headers</span></span>
|<span data-ttu-id="ddd4a-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ddd4a-117">Header</span></span>|<span data-ttu-id="ddd4a-118">Значение</span><span class="sxs-lookup"><span data-stu-id="ddd4a-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ddd4a-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="ddd4a-119">Authorization</span></span>|<span data-ttu-id="ddd4a-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ddd4a-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ddd4a-121">Accept</span><span class="sxs-lookup"><span data-stu-id="ddd4a-121">Accept</span></span>|<span data-ttu-id="ddd4a-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ddd4a-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ddd4a-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ddd4a-123">Request body</span></span>
<span data-ttu-id="ddd4a-124">В теле запроса добавьте представление объекта [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ddd4a-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_apps_windowsuniversalappx.md) object.</span></span>

<span data-ttu-id="ddd4a-125">Ниже показаны свойства, которые необходимо указывать при создании объекта [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="ddd4a-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="ddd4a-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="ddd4a-126">Property</span></span>|<span data-ttu-id="ddd4a-127">Тип</span><span class="sxs-lookup"><span data-stu-id="ddd4a-127">Type</span></span>|<span data-ttu-id="ddd4a-128">Описание</span><span class="sxs-lookup"><span data-stu-id="ddd4a-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddd4a-129">id</span><span class="sxs-lookup"><span data-stu-id="ddd4a-129">id</span></span>|<span data-ttu-id="ddd4a-130">String</span><span class="sxs-lookup"><span data-stu-id="ddd4a-130">String</span></span>|<span data-ttu-id="ddd4a-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ddd4a-131">Key of the setting.</span></span> <span data-ttu-id="ddd4a-132">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ddd4a-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ddd4a-133">displayName</span><span class="sxs-lookup"><span data-stu-id="ddd4a-133">displayName</span></span>|<span data-ttu-id="ddd4a-134">String</span><span class="sxs-lookup"><span data-stu-id="ddd4a-134">String</span></span>|<span data-ttu-id="ddd4a-135">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="ddd4a-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ddd4a-136">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ddd4a-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ddd4a-137">description</span><span class="sxs-lookup"><span data-stu-id="ddd4a-137">description</span></span>|<span data-ttu-id="ddd4a-138">String</span><span class="sxs-lookup"><span data-stu-id="ddd4a-138">String</span></span>|<span data-ttu-id="ddd4a-139">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="ddd4a-139">The description of the app.</span></span> <span data-ttu-id="ddd4a-140">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ddd4a-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ddd4a-141">publisher</span><span class="sxs-lookup"><span data-stu-id="ddd4a-141">Publisher</span></span>|<span data-ttu-id="ddd4a-142">String</span><span class="sxs-lookup"><span data-stu-id="ddd4a-142">String</span></span>|<span data-ttu-id="ddd4a-143">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="ddd4a-143">The name of the app.</span></span> <span data-ttu-id="ddd4a-144">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ddd4a-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ddd4a-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ddd4a-145">largeIcon</span></span>|[<span data-ttu-id="ddd4a-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ddd4a-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="ddd4a-147">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="ddd4a-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ddd4a-148">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ddd4a-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ddd4a-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ddd4a-149">createdDateTime</span></span>|<span data-ttu-id="ddd4a-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ddd4a-150">DateTimeOffset</span></span>|<span data-ttu-id="ddd4a-151">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="ddd4a-151">The date and time the group was created.</span></span> <span data-ttu-id="ddd4a-152">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ddd4a-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ddd4a-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ddd4a-153">lastModifiedDateTime</span></span>|<span data-ttu-id="ddd4a-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ddd4a-154">DateTimeOffset</span></span>|<span data-ttu-id="ddd4a-155">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="ddd4a-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="ddd4a-156">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ddd4a-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ddd4a-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ddd4a-157">isFeatured</span></span>|<span data-ttu-id="ddd4a-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddd4a-158">Boolean</span></span>|<span data-ttu-id="ddd4a-159">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ddd4a-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ddd4a-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ddd4a-160">privacyInformationUrl</span></span>|<span data-ttu-id="ddd4a-161">String</span><span class="sxs-lookup"><span data-stu-id="ddd4a-161">String</span></span>|<span data-ttu-id="ddd4a-162">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="ddd4a-162">The privacy statement Url.</span></span> <span data-ttu-id="ddd4a-163">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ddd4a-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ddd4a-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ddd4a-164">informationUrl</span></span>|<span data-ttu-id="ddd4a-165">String</span><span class="sxs-lookup"><span data-stu-id="ddd4a-165">String</span></span>|<span data-ttu-id="ddd4a-166">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="ddd4a-166">The more information Url.</span></span> <span data-ttu-id="ddd4a-167">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ddd4a-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ddd4a-168">owner</span><span class="sxs-lookup"><span data-stu-id="ddd4a-168">owner</span></span>|<span data-ttu-id="ddd4a-169">String</span><span class="sxs-lookup"><span data-stu-id="ddd4a-169">String</span></span>|<span data-ttu-id="ddd4a-170">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="ddd4a-170">The owner of the app.</span></span> <span data-ttu-id="ddd4a-171">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ddd4a-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ddd4a-172">developer</span><span class="sxs-lookup"><span data-stu-id="ddd4a-172">developer</span></span>|<span data-ttu-id="ddd4a-173">String</span><span class="sxs-lookup"><span data-stu-id="ddd4a-173">String</span></span>|<span data-ttu-id="ddd4a-174">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="ddd4a-174">The name of the app.</span></span> <span data-ttu-id="ddd4a-175">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ddd4a-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ddd4a-176">notes</span><span class="sxs-lookup"><span data-stu-id="ddd4a-176">Notes</span></span>|<span data-ttu-id="ddd4a-177">String</span><span class="sxs-lookup"><span data-stu-id="ddd4a-177">String</span></span>|<span data-ttu-id="ddd4a-178">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="ddd4a-178">Notes for the app.</span></span> <span data-ttu-id="ddd4a-179">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ddd4a-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ddd4a-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="ddd4a-180">publishingState</span></span>|<span data-ttu-id="ddd4a-181">String</span><span class="sxs-lookup"><span data-stu-id="ddd4a-181">String</span></span>|<span data-ttu-id="ddd4a-182">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="ddd4a-182">The publishing state for the app.</span></span> <span data-ttu-id="ddd4a-183">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="ddd4a-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ddd4a-184">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md). Допустимые значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="ddd4a-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ddd4a-185">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="ddd4a-185">committedContentVersion</span></span>|<span data-ttu-id="ddd4a-186">String</span><span class="sxs-lookup"><span data-stu-id="ddd4a-186">String</span></span>|<span data-ttu-id="ddd4a-187">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="ddd4a-187">The internal committed content version.</span></span> <span data-ttu-id="ddd4a-188">Наследуется от [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ddd4a-188">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="ddd4a-189">fileName</span><span class="sxs-lookup"><span data-stu-id="ddd4a-189">fileName</span></span>|<span data-ttu-id="ddd4a-190">String</span><span class="sxs-lookup"><span data-stu-id="ddd4a-190">String</span></span>|<span data-ttu-id="ddd4a-191">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="ddd4a-191">The name of the main Lob application file.</span></span> <span data-ttu-id="ddd4a-192">Наследуется от [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ddd4a-192">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="ddd4a-193">size</span><span class="sxs-lookup"><span data-stu-id="ddd4a-193">size</span></span>|<span data-ttu-id="ddd4a-194">Int64</span><span class="sxs-lookup"><span data-stu-id="ddd4a-194">Int64</span></span>|<span data-ttu-id="ddd4a-195">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="ddd4a-195">The total size, including all uploaded files.</span></span> <span data-ttu-id="ddd4a-196">Наследуется от [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ddd4a-196">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="ddd4a-197">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="ddd4a-197">applicableArchitectures</span></span>|<span data-ttu-id="ddd4a-198">String</span><span class="sxs-lookup"><span data-stu-id="ddd4a-198">String</span></span>|<span data-ttu-id="ddd4a-199">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="ddd4a-199">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="ddd4a-200">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="ddd4a-200">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="ddd4a-201">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="ddd4a-201">applicableDeviceTypes</span></span>|<span data-ttu-id="ddd4a-202">String</span><span class="sxs-lookup"><span data-stu-id="ddd4a-202">String</span></span>|<span data-ttu-id="ddd4a-203">Типы устройств с Windows, которые поддерживаются этим приложением.</span><span class="sxs-lookup"><span data-stu-id="ddd4a-203">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="ddd4a-204">Возможные значения: `none`, `desktop`, `mobile`, `holographic`, `team`.</span><span class="sxs-lookup"><span data-stu-id="ddd4a-204">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="ddd4a-205">identityName</span><span class="sxs-lookup"><span data-stu-id="ddd4a-205">identityName</span></span>|<span data-ttu-id="ddd4a-206">String</span><span class="sxs-lookup"><span data-stu-id="ddd4a-206">String</span></span>|<span data-ttu-id="ddd4a-207">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="ddd4a-207">The Identity Name.</span></span>|
|<span data-ttu-id="ddd4a-208">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="ddd4a-208">identityPublisherHash</span></span>|<span data-ttu-id="ddd4a-209">String</span><span class="sxs-lookup"><span data-stu-id="ddd4a-209">String</span></span>|<span data-ttu-id="ddd4a-210">Хэш издателей удостоверений.</span><span class="sxs-lookup"><span data-stu-id="ddd4a-210">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="ddd4a-211">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="ddd4a-211">identityResourceIdentifier</span></span>|<span data-ttu-id="ddd4a-212">String</span><span class="sxs-lookup"><span data-stu-id="ddd4a-212">String</span></span>|<span data-ttu-id="ddd4a-213">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="ddd4a-213">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="ddd4a-214">isBundle</span><span class="sxs-lookup"><span data-stu-id="ddd4a-214">isBundle</span></span>|<span data-ttu-id="ddd4a-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddd4a-215">Boolean</span></span>|<span data-ttu-id="ddd4a-216">Указывает, является ли приложение пакетом.</span><span class="sxs-lookup"><span data-stu-id="ddd4a-216">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="ddd4a-217">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ddd4a-217">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="ddd4a-218">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ddd4a-218">windowsMinimumOperatingSystem</span></span>](../resources/intune_apps_windowsminimumoperatingsystem.md)|<span data-ttu-id="ddd4a-219">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="ddd4a-219">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="ddd4a-220">identityVersion</span><span class="sxs-lookup"><span data-stu-id="ddd4a-220">identityVersion</span></span>|<span data-ttu-id="ddd4a-221">String</span><span class="sxs-lookup"><span data-stu-id="ddd4a-221">String</span></span>|<span data-ttu-id="ddd4a-222">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="ddd4a-222">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="ddd4a-223">Ответ</span><span class="sxs-lookup"><span data-stu-id="ddd4a-223">Response</span></span>
<span data-ttu-id="ddd4a-224">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ddd4a-224">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_apps_windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ddd4a-225">Пример</span><span class="sxs-lookup"><span data-stu-id="ddd4a-225">Example</span></span>
### <a name="request"></a><span data-ttu-id="ddd4a-226">Запрос</span><span class="sxs-lookup"><span data-stu-id="ddd4a-226">Request</span></span>
<span data-ttu-id="ddd4a-227">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ddd4a-227">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1194

{
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

### <a name="response"></a><span data-ttu-id="ddd4a-228">Ответ</span><span class="sxs-lookup"><span data-stu-id="ddd4a-228">Response</span></span>
<span data-ttu-id="ddd4a-p120">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ddd4a-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



