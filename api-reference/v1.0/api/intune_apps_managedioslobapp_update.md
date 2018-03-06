# <a name="update-managedioslobapp"></a><span data-ttu-id="bda61-101">Update managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="bda61-101">Update managedIOSLobApp</span></span>

> <span data-ttu-id="bda61-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bda61-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bda61-103">Обновление свойств объекта [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="bda61-103">Update the properties of a [calendar](../resources/intune_apps_managedioslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bda61-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="bda61-104">Prerequisites</span></span>
<span data-ttu-id="bda61-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bda61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bda61-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bda61-107">Permission type</span></span>|<span data-ttu-id="bda61-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bda61-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bda61-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bda61-109">Delegated (work or school account)</span></span>|<span data-ttu-id="bda61-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bda61-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bda61-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bda61-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bda61-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bda61-112">Not supported.</span></span>|
|<span data-ttu-id="bda61-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bda61-113">Application</span></span>|<span data-ttu-id="bda61-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bda61-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bda61-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bda61-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="bda61-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bda61-116">Request headers</span></span>
|<span data-ttu-id="bda61-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bda61-117">Header</span></span>|<span data-ttu-id="bda61-118">Значение</span><span class="sxs-lookup"><span data-stu-id="bda61-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bda61-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="bda61-119">Authorization</span></span>|<span data-ttu-id="bda61-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bda61-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="bda61-121">Accept</span><span class="sxs-lookup"><span data-stu-id="bda61-121">Accept</span></span>|<span data-ttu-id="bda61-122">application/json</span><span class="sxs-lookup"><span data-stu-id="bda61-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bda61-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bda61-123">Request body</span></span>
<span data-ttu-id="bda61-124">В теле запроса добавьте представление объекта [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bda61-124">In the request body, supply a JSON representation of [Attachment](../resources/intune_apps_managedioslobapp.md) object.</span></span>

<span data-ttu-id="bda61-125">Ниже показаны свойства, которые необходимо указывать при создании объекта [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="bda61-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="bda61-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="bda61-126">Property</span></span>|<span data-ttu-id="bda61-127">Тип</span><span class="sxs-lookup"><span data-stu-id="bda61-127">Type</span></span>|<span data-ttu-id="bda61-128">Описание</span><span class="sxs-lookup"><span data-stu-id="bda61-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bda61-129">id</span><span class="sxs-lookup"><span data-stu-id="bda61-129">id</span></span>|<span data-ttu-id="bda61-130">String</span><span class="sxs-lookup"><span data-stu-id="bda61-130">String</span></span>|<span data-ttu-id="bda61-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bda61-131">Key of the setting.</span></span> <span data-ttu-id="bda61-132">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bda61-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="bda61-133">displayName</span><span class="sxs-lookup"><span data-stu-id="bda61-133">displayName</span></span>|<span data-ttu-id="bda61-134">String</span><span class="sxs-lookup"><span data-stu-id="bda61-134">String</span></span>|<span data-ttu-id="bda61-135">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="bda61-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="bda61-136">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bda61-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="bda61-137">description</span><span class="sxs-lookup"><span data-stu-id="bda61-137">description</span></span>|<span data-ttu-id="bda61-138">String</span><span class="sxs-lookup"><span data-stu-id="bda61-138">String</span></span>|<span data-ttu-id="bda61-139">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="bda61-139">The description of the app.</span></span> <span data-ttu-id="bda61-140">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bda61-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="bda61-141">publisher</span><span class="sxs-lookup"><span data-stu-id="bda61-141">Publisher</span></span>|<span data-ttu-id="bda61-142">String</span><span class="sxs-lookup"><span data-stu-id="bda61-142">String</span></span>|<span data-ttu-id="bda61-143">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="bda61-143">The name of the app.</span></span> <span data-ttu-id="bda61-144">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bda61-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="bda61-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="bda61-145">largeIcon</span></span>|[<span data-ttu-id="bda61-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="bda61-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="bda61-147">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="bda61-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="bda61-148">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bda61-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="bda61-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bda61-149">createdDateTime</span></span>|<span data-ttu-id="bda61-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bda61-150">DateTimeOffset</span></span>|<span data-ttu-id="bda61-151">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="bda61-151">The date and time the group was created.</span></span> <span data-ttu-id="bda61-152">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bda61-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="bda61-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bda61-153">lastModifiedDateTime</span></span>|<span data-ttu-id="bda61-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bda61-154">DateTimeOffset</span></span>|<span data-ttu-id="bda61-155">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="bda61-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="bda61-156">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bda61-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="bda61-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="bda61-157">isFeatured</span></span>|<span data-ttu-id="bda61-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="bda61-158">Boolean</span></span>|<span data-ttu-id="bda61-159">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bda61-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="bda61-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="bda61-160">privacyInformationUrl</span></span>|<span data-ttu-id="bda61-161">String</span><span class="sxs-lookup"><span data-stu-id="bda61-161">String</span></span>|<span data-ttu-id="bda61-162">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="bda61-162">The privacy statement Url.</span></span> <span data-ttu-id="bda61-163">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bda61-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="bda61-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="bda61-164">informationUrl</span></span>|<span data-ttu-id="bda61-165">String</span><span class="sxs-lookup"><span data-stu-id="bda61-165">String</span></span>|<span data-ttu-id="bda61-166">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="bda61-166">The more information Url.</span></span> <span data-ttu-id="bda61-167">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bda61-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="bda61-168">owner</span><span class="sxs-lookup"><span data-stu-id="bda61-168">owner</span></span>|<span data-ttu-id="bda61-169">String</span><span class="sxs-lookup"><span data-stu-id="bda61-169">String</span></span>|<span data-ttu-id="bda61-170">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="bda61-170">The owner of the app.</span></span> <span data-ttu-id="bda61-171">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bda61-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="bda61-172">developer</span><span class="sxs-lookup"><span data-stu-id="bda61-172">developer</span></span>|<span data-ttu-id="bda61-173">String</span><span class="sxs-lookup"><span data-stu-id="bda61-173">String</span></span>|<span data-ttu-id="bda61-174">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="bda61-174">The name of the app.</span></span> <span data-ttu-id="bda61-175">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bda61-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="bda61-176">notes</span><span class="sxs-lookup"><span data-stu-id="bda61-176">Notes</span></span>|<span data-ttu-id="bda61-177">String</span><span class="sxs-lookup"><span data-stu-id="bda61-177">String</span></span>|<span data-ttu-id="bda61-178">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="bda61-178">Notes for the app.</span></span> <span data-ttu-id="bda61-179">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bda61-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="bda61-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="bda61-180">publishingState</span></span>|<span data-ttu-id="bda61-181">String</span><span class="sxs-lookup"><span data-stu-id="bda61-181">String</span></span>|<span data-ttu-id="bda61-182">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="bda61-182">The publishing state for the app.</span></span> <span data-ttu-id="bda61-183">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="bda61-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="bda61-184">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md). Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="bda61-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="bda61-185">appAvailability</span><span class="sxs-lookup"><span data-stu-id="bda61-185">appAvailability</span></span>|<span data-ttu-id="bda61-186">String</span><span class="sxs-lookup"><span data-stu-id="bda61-186">String</span></span>|<span data-ttu-id="bda61-187">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="bda61-187">The Application's availability.</span></span> <span data-ttu-id="bda61-188">Наследуется от объекта [managedApp](../resources/intune_apps_managedapp.md). Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="bda61-188">Inherited from [managedApp](../resources/intune_apps_managedapp.md) Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="bda61-189">version</span><span class="sxs-lookup"><span data-stu-id="bda61-189">version</span></span>|<span data-ttu-id="bda61-190">String</span><span class="sxs-lookup"><span data-stu-id="bda61-190">String</span></span>|<span data-ttu-id="bda61-191">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="bda61-191">The Application's version.</span></span> <span data-ttu-id="bda61-192">Наследуется от объекта [managedApp](../resources/intune_apps_managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="bda61-192">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="bda61-193">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="bda61-193">committedContentVersion</span></span>|<span data-ttu-id="bda61-194">String</span><span class="sxs-lookup"><span data-stu-id="bda61-194">String</span></span>|<span data-ttu-id="bda61-195">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="bda61-195">The internal committed content version.</span></span> <span data-ttu-id="bda61-196">Наследуется от [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="bda61-196">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="bda61-197">fileName</span><span class="sxs-lookup"><span data-stu-id="bda61-197">fileName</span></span>|<span data-ttu-id="bda61-198">String</span><span class="sxs-lookup"><span data-stu-id="bda61-198">String</span></span>|<span data-ttu-id="bda61-199">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="bda61-199">The name of the main Lob application file.</span></span> <span data-ttu-id="bda61-200">Наследуется от [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="bda61-200">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="bda61-201">size</span><span class="sxs-lookup"><span data-stu-id="bda61-201">size</span></span>|<span data-ttu-id="bda61-202">Int64</span><span class="sxs-lookup"><span data-stu-id="bda61-202">Int64</span></span>|<span data-ttu-id="bda61-203">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="bda61-203">The total size, including all uploaded files.</span></span> <span data-ttu-id="bda61-204">Наследуется от [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="bda61-204">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="bda61-205">bundleId</span><span class="sxs-lookup"><span data-stu-id="bda61-205">bundleId</span></span>|<span data-ttu-id="bda61-206">String</span><span class="sxs-lookup"><span data-stu-id="bda61-206">String</span></span>|<span data-ttu-id="bda61-207">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="bda61-207">The Identity Name.</span></span>|
|<span data-ttu-id="bda61-208">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="bda61-208">applicableDeviceType</span></span>|[<span data-ttu-id="bda61-209">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="bda61-209">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="bda61-210">Архитектура iOS, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="bda61-210">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="bda61-211">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="bda61-211">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="bda61-212">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="bda61-212">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="bda61-213">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="bda61-213">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="bda61-214">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="bda61-214">expirationDateTime</span></span>|<span data-ttu-id="bda61-215">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bda61-215">DateTimeOffset</span></span>|<span data-ttu-id="bda61-216">Срок действия.</span><span class="sxs-lookup"><span data-stu-id="bda61-216">: The expiration time for the subscription.</span></span>|
|<span data-ttu-id="bda61-217">versionNumber</span><span class="sxs-lookup"><span data-stu-id="bda61-217">versionNumber</span></span>|<span data-ttu-id="bda61-218">String</span><span class="sxs-lookup"><span data-stu-id="bda61-218">String</span></span>|<span data-ttu-id="bda61-219">Номер версии управляемого бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="bda61-219">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="bda61-220">buildNumber</span><span class="sxs-lookup"><span data-stu-id="bda61-220">buildNumber</span></span>|<span data-ttu-id="bda61-221">String</span><span class="sxs-lookup"><span data-stu-id="bda61-221">String</span></span>|<span data-ttu-id="bda61-222">Номер сборки управляемого бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="bda61-222">The build number of managed iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="bda61-223">Ответ</span><span class="sxs-lookup"><span data-stu-id="bda61-223">Response</span></span>
<span data-ttu-id="bda61-224">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="bda61-224">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_apps_managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bda61-225">Пример</span><span class="sxs-lookup"><span data-stu-id="bda61-225">Example</span></span>
### <a name="request"></a><span data-ttu-id="bda61-226">Запрос</span><span class="sxs-lookup"><span data-stu-id="bda61-226">Request</span></span>
<span data-ttu-id="bda61-227">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bda61-227">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1276

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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```

### <a name="response"></a><span data-ttu-id="bda61-228">Ответ</span><span class="sxs-lookup"><span data-stu-id="bda61-228">Response</span></span>
<span data-ttu-id="bda61-p120">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bda61-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1439

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
  "id": "8f59792d-792d-8f59-2d79-598f2d79598f",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```



