# <a name="create-managedioslobapp"></a><span data-ttu-id="cc6a0-101">Create managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="cc6a0-101">Create managedIOSLobApp</span></span>

> <span data-ttu-id="cc6a0-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="cc6a0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cc6a0-103">Создание объекта [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc6a0-103">Create a new [plannerBucket](../resources/intune_apps_managedioslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cc6a0-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="cc6a0-104">Prerequisites</span></span>
<span data-ttu-id="cc6a0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cc6a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cc6a0-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cc6a0-107">Permission type</span></span>|<span data-ttu-id="cc6a0-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cc6a0-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cc6a0-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cc6a0-109">Delegated (work or school account)</span></span>|<span data-ttu-id="cc6a0-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc6a0-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cc6a0-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cc6a0-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc6a0-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc6a0-112">Not supported.</span></span>|
|<span data-ttu-id="cc6a0-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cc6a0-113">Application</span></span>|<span data-ttu-id="cc6a0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc6a0-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc6a0-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cc6a0-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="cc6a0-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cc6a0-116">Request headers</span></span>
|<span data-ttu-id="cc6a0-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cc6a0-117">Header</span></span>|<span data-ttu-id="cc6a0-118">Значение</span><span class="sxs-lookup"><span data-stu-id="cc6a0-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cc6a0-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc6a0-119">Authorization</span></span>|<span data-ttu-id="cc6a0-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cc6a0-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="cc6a0-121">Accept</span><span class="sxs-lookup"><span data-stu-id="cc6a0-121">Accept</span></span>|<span data-ttu-id="cc6a0-122">application/json</span><span class="sxs-lookup"><span data-stu-id="cc6a0-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc6a0-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cc6a0-123">Request body</span></span>
<span data-ttu-id="cc6a0-124">В тексте запроса добавьте представление объекта managedIOSLobApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cc6a0-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="cc6a0-125">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта managedIOSLobApp.</span><span class="sxs-lookup"><span data-stu-id="cc6a0-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="cc6a0-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="cc6a0-126">Property</span></span>|<span data-ttu-id="cc6a0-127">Тип</span><span class="sxs-lookup"><span data-stu-id="cc6a0-127">Type</span></span>|<span data-ttu-id="cc6a0-128">Описание</span><span class="sxs-lookup"><span data-stu-id="cc6a0-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc6a0-129">id</span><span class="sxs-lookup"><span data-stu-id="cc6a0-129">id</span></span>|<span data-ttu-id="cc6a0-130">String</span><span class="sxs-lookup"><span data-stu-id="cc6a0-130">String</span></span>|<span data-ttu-id="cc6a0-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="cc6a0-131">Key of the setting.</span></span> <span data-ttu-id="cc6a0-132">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc6a0-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cc6a0-133">displayName</span><span class="sxs-lookup"><span data-stu-id="cc6a0-133">displayName</span></span>|<span data-ttu-id="cc6a0-134">String</span><span class="sxs-lookup"><span data-stu-id="cc6a0-134">String</span></span>|<span data-ttu-id="cc6a0-135">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="cc6a0-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="cc6a0-136">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc6a0-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cc6a0-137">description</span><span class="sxs-lookup"><span data-stu-id="cc6a0-137">description</span></span>|<span data-ttu-id="cc6a0-138">String</span><span class="sxs-lookup"><span data-stu-id="cc6a0-138">String</span></span>|<span data-ttu-id="cc6a0-139">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="cc6a0-139">The description of the app.</span></span> <span data-ttu-id="cc6a0-140">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc6a0-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cc6a0-141">publisher</span><span class="sxs-lookup"><span data-stu-id="cc6a0-141">Publisher</span></span>|<span data-ttu-id="cc6a0-142">String</span><span class="sxs-lookup"><span data-stu-id="cc6a0-142">String</span></span>|<span data-ttu-id="cc6a0-143">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="cc6a0-143">The name of the app.</span></span> <span data-ttu-id="cc6a0-144">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc6a0-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cc6a0-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="cc6a0-145">largeIcon</span></span>|[<span data-ttu-id="cc6a0-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="cc6a0-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="cc6a0-147">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="cc6a0-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="cc6a0-148">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc6a0-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cc6a0-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cc6a0-149">createdDateTime</span></span>|<span data-ttu-id="cc6a0-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc6a0-150">DateTimeOffset</span></span>|<span data-ttu-id="cc6a0-151">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="cc6a0-151">The date and time the group was created.</span></span> <span data-ttu-id="cc6a0-152">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc6a0-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cc6a0-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cc6a0-153">lastModifiedDateTime</span></span>|<span data-ttu-id="cc6a0-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc6a0-154">DateTimeOffset</span></span>|<span data-ttu-id="cc6a0-155">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="cc6a0-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="cc6a0-156">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc6a0-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cc6a0-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="cc6a0-157">isFeatured</span></span>|<span data-ttu-id="cc6a0-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc6a0-158">Boolean</span></span>|<span data-ttu-id="cc6a0-159">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc6a0-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cc6a0-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="cc6a0-160">privacyInformationUrl</span></span>|<span data-ttu-id="cc6a0-161">String</span><span class="sxs-lookup"><span data-stu-id="cc6a0-161">String</span></span>|<span data-ttu-id="cc6a0-162">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="cc6a0-162">The privacy statement Url.</span></span> <span data-ttu-id="cc6a0-163">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc6a0-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cc6a0-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="cc6a0-164">informationUrl</span></span>|<span data-ttu-id="cc6a0-165">String</span><span class="sxs-lookup"><span data-stu-id="cc6a0-165">String</span></span>|<span data-ttu-id="cc6a0-166">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="cc6a0-166">The more information Url.</span></span> <span data-ttu-id="cc6a0-167">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc6a0-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cc6a0-168">owner</span><span class="sxs-lookup"><span data-stu-id="cc6a0-168">owner</span></span>|<span data-ttu-id="cc6a0-169">String</span><span class="sxs-lookup"><span data-stu-id="cc6a0-169">String</span></span>|<span data-ttu-id="cc6a0-170">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="cc6a0-170">The owner of the app.</span></span> <span data-ttu-id="cc6a0-171">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc6a0-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cc6a0-172">developer</span><span class="sxs-lookup"><span data-stu-id="cc6a0-172">developer</span></span>|<span data-ttu-id="cc6a0-173">String</span><span class="sxs-lookup"><span data-stu-id="cc6a0-173">String</span></span>|<span data-ttu-id="cc6a0-174">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="cc6a0-174">The name of the app.</span></span> <span data-ttu-id="cc6a0-175">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc6a0-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cc6a0-176">notes</span><span class="sxs-lookup"><span data-stu-id="cc6a0-176">Notes</span></span>|<span data-ttu-id="cc6a0-177">String</span><span class="sxs-lookup"><span data-stu-id="cc6a0-177">String</span></span>|<span data-ttu-id="cc6a0-178">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="cc6a0-178">Notes for the app.</span></span> <span data-ttu-id="cc6a0-179">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc6a0-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cc6a0-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="cc6a0-180">publishingState</span></span>|<span data-ttu-id="cc6a0-181">String</span><span class="sxs-lookup"><span data-stu-id="cc6a0-181">String</span></span>|<span data-ttu-id="cc6a0-182">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="cc6a0-182">The publishing state for the app.</span></span> <span data-ttu-id="cc6a0-183">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="cc6a0-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="cc6a0-184">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md). Допустимые значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="cc6a0-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="cc6a0-185">appAvailability</span><span class="sxs-lookup"><span data-stu-id="cc6a0-185">appAvailability</span></span>|<span data-ttu-id="cc6a0-186">String</span><span class="sxs-lookup"><span data-stu-id="cc6a0-186">String</span></span>|<span data-ttu-id="cc6a0-187">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="cc6a0-187">The Application's availability.</span></span> <span data-ttu-id="cc6a0-188">Наследуется от объекта [managedApp](../resources/intune_apps_managedapp.md). Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="cc6a0-188">Inherited from [managedApp](../resources/intune_apps_managedapp.md) Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="cc6a0-189">version</span><span class="sxs-lookup"><span data-stu-id="cc6a0-189">version</span></span>|<span data-ttu-id="cc6a0-190">String</span><span class="sxs-lookup"><span data-stu-id="cc6a0-190">String</span></span>|<span data-ttu-id="cc6a0-191">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="cc6a0-191">The Application's version.</span></span> <span data-ttu-id="cc6a0-192">Наследуется от объекта [managedApp](../resources/intune_apps_managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc6a0-192">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="cc6a0-193">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="cc6a0-193">committedContentVersion</span></span>|<span data-ttu-id="cc6a0-194">String</span><span class="sxs-lookup"><span data-stu-id="cc6a0-194">String</span></span>|<span data-ttu-id="cc6a0-195">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="cc6a0-195">The internal committed content version.</span></span> <span data-ttu-id="cc6a0-196">Наследуется от объекта [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc6a0-196">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="cc6a0-197">fileName</span><span class="sxs-lookup"><span data-stu-id="cc6a0-197">fileName</span></span>|<span data-ttu-id="cc6a0-198">String</span><span class="sxs-lookup"><span data-stu-id="cc6a0-198">String</span></span>|<span data-ttu-id="cc6a0-199">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="cc6a0-199">The name of the main Lob application file.</span></span> <span data-ttu-id="cc6a0-200">Наследуется от объекта [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc6a0-200">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="cc6a0-201">size</span><span class="sxs-lookup"><span data-stu-id="cc6a0-201">size</span></span>|<span data-ttu-id="cc6a0-202">Int64</span><span class="sxs-lookup"><span data-stu-id="cc6a0-202">Int64</span></span>|<span data-ttu-id="cc6a0-203">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="cc6a0-203">The total size, including all uploaded files.</span></span> <span data-ttu-id="cc6a0-204">Наследуется от объекта [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc6a0-204">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="cc6a0-205">bundleId</span><span class="sxs-lookup"><span data-stu-id="cc6a0-205">bundleId</span></span>|<span data-ttu-id="cc6a0-206">String</span><span class="sxs-lookup"><span data-stu-id="cc6a0-206">String</span></span>|<span data-ttu-id="cc6a0-207">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="cc6a0-207">The Identity Name.</span></span>|
|<span data-ttu-id="cc6a0-208">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="cc6a0-208">applicableDeviceType</span></span>|[<span data-ttu-id="cc6a0-209">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="cc6a0-209">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="cc6a0-210">Архитектура iOS, поддерживаемая этим приложением.</span><span class="sxs-lookup"><span data-stu-id="cc6a0-210">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="cc6a0-211">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="cc6a0-211">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="cc6a0-212">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="cc6a0-212">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="cc6a0-213">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="cc6a0-213">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="cc6a0-214">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="cc6a0-214">expirationDateTime</span></span>|<span data-ttu-id="cc6a0-215">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc6a0-215">DateTimeOffset</span></span>|<span data-ttu-id="cc6a0-216">Время окончания срока действия.</span><span class="sxs-lookup"><span data-stu-id="cc6a0-216">: The expiration time for the subscription.</span></span>|
|<span data-ttu-id="cc6a0-217">versionNumber</span><span class="sxs-lookup"><span data-stu-id="cc6a0-217">versionNumber</span></span>|<span data-ttu-id="cc6a0-218">String</span><span class="sxs-lookup"><span data-stu-id="cc6a0-218">String</span></span>|<span data-ttu-id="cc6a0-219">Номер версии управляемого бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="cc6a0-219">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="cc6a0-220">buildNumber</span><span class="sxs-lookup"><span data-stu-id="cc6a0-220">buildNumber</span></span>|<span data-ttu-id="cc6a0-221">String</span><span class="sxs-lookup"><span data-stu-id="cc6a0-221">String</span></span>|<span data-ttu-id="cc6a0-222">Номер сборки управляемого бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="cc6a0-222">The build number of managed iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="cc6a0-223">Ответ</span><span class="sxs-lookup"><span data-stu-id="cc6a0-223">Response</span></span>
<span data-ttu-id="cc6a0-224">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="cc6a0-224">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_apps_managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc6a0-225">Пример</span><span class="sxs-lookup"><span data-stu-id="cc6a0-225">Example</span></span>
### <a name="request"></a><span data-ttu-id="cc6a0-226">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc6a0-226">Request</span></span>
<span data-ttu-id="cc6a0-227">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cc6a0-227">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1331

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
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

### <a name="response"></a><span data-ttu-id="cc6a0-228">Ответ</span><span class="sxs-lookup"><span data-stu-id="cc6a0-228">Response</span></span>
<span data-ttu-id="cc6a0-p120">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="cc6a0-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



