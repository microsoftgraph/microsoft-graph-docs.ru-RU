# <a name="create-managedioslobapp"></a><span data-ttu-id="fcd5a-101">Создание managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="fcd5a-101">Create managedIOSLobApp</span></span>

> <span data-ttu-id="fcd5a-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fcd5a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fcd5a-103">Создание объекта [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="fcd5a-103">Create a new [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fcd5a-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="fcd5a-104">Prerequisites</span></span>
<span data-ttu-id="fcd5a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fcd5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fcd5a-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fcd5a-107">Permission type</span></span>|<span data-ttu-id="fcd5a-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fcd5a-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fcd5a-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fcd5a-109">Delegated (work or school account)</span></span>|<span data-ttu-id="fcd5a-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcd5a-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fcd5a-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fcd5a-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fcd5a-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcd5a-112">Not supported.</span></span>|
|<span data-ttu-id="fcd5a-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fcd5a-113">Application</span></span>|<span data-ttu-id="fcd5a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcd5a-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fcd5a-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fcd5a-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="fcd5a-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fcd5a-116">Request headers</span></span>
|<span data-ttu-id="fcd5a-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fcd5a-117">Header</span></span>|<span data-ttu-id="fcd5a-118">Значение</span><span class="sxs-lookup"><span data-stu-id="fcd5a-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fcd5a-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fcd5a-119">Authorization</span></span>|<span data-ttu-id="fcd5a-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="fcd5a-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fcd5a-121">Принять</span><span class="sxs-lookup"><span data-stu-id="fcd5a-121">Accept</span></span>|<span data-ttu-id="fcd5a-122">application/json</span><span class="sxs-lookup"><span data-stu-id="fcd5a-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fcd5a-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fcd5a-123">Request body</span></span>
<span data-ttu-id="fcd5a-124">В тексте запроса добавьте представление объекта managedIOSLobApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fcd5a-124">In the request body, supply a JSON representation for the managedIOSLobApp object.</span></span>

<span data-ttu-id="fcd5a-125">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта managedIOSLobApp.</span><span class="sxs-lookup"><span data-stu-id="fcd5a-125">The following table shows the properties that are required when you create the managedIOSLobApp.</span></span>

|<span data-ttu-id="fcd5a-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="fcd5a-126">Property</span></span>|<span data-ttu-id="fcd5a-127">Тип</span><span class="sxs-lookup"><span data-stu-id="fcd5a-127">Type</span></span>|<span data-ttu-id="fcd5a-128">Описание</span><span class="sxs-lookup"><span data-stu-id="fcd5a-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fcd5a-129">id</span><span class="sxs-lookup"><span data-stu-id="fcd5a-129">id</span></span>|<span data-ttu-id="fcd5a-130">Строка</span><span class="sxs-lookup"><span data-stu-id="fcd5a-130">String</span></span>|<span data-ttu-id="fcd5a-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fcd5a-131">Key of the entity.</span></span> <span data-ttu-id="fcd5a-132">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fcd5a-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fcd5a-133">displayName</span><span class="sxs-lookup"><span data-stu-id="fcd5a-133">displayName</span></span>|<span data-ttu-id="fcd5a-134">Строка</span><span class="sxs-lookup"><span data-stu-id="fcd5a-134">String</span></span>|<span data-ttu-id="fcd5a-135">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="fcd5a-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="fcd5a-136">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fcd5a-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fcd5a-137">description</span><span class="sxs-lookup"><span data-stu-id="fcd5a-137">description</span></span>|<span data-ttu-id="fcd5a-138">Строка</span><span class="sxs-lookup"><span data-stu-id="fcd5a-138">String</span></span>|<span data-ttu-id="fcd5a-139">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="fcd5a-139">The description of the app.</span></span> <span data-ttu-id="fcd5a-140">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fcd5a-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fcd5a-141">publisher</span><span class="sxs-lookup"><span data-stu-id="fcd5a-141">publisher</span></span>|<span data-ttu-id="fcd5a-142">Строка</span><span class="sxs-lookup"><span data-stu-id="fcd5a-142">String</span></span>|<span data-ttu-id="fcd5a-143">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="fcd5a-143">The publisher of the app.</span></span> <span data-ttu-id="fcd5a-144">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fcd5a-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fcd5a-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="fcd5a-145">largeIcon</span></span>|[<span data-ttu-id="fcd5a-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="fcd5a-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="fcd5a-147">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="fcd5a-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="fcd5a-148">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fcd5a-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fcd5a-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fcd5a-149">createdDateTime</span></span>|<span data-ttu-id="fcd5a-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fcd5a-150">DateTimeOffset</span></span>|<span data-ttu-id="fcd5a-151">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="fcd5a-151">The date and time the app was created.</span></span> <span data-ttu-id="fcd5a-152">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fcd5a-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fcd5a-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fcd5a-153">lastModifiedDateTime</span></span>|<span data-ttu-id="fcd5a-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fcd5a-154">DateTimeOffset</span></span>|<span data-ttu-id="fcd5a-155">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="fcd5a-155">The date and time the app was last modified.</span></span> <span data-ttu-id="fcd5a-156">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fcd5a-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fcd5a-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="fcd5a-157">isFeatured</span></span>|<span data-ttu-id="fcd5a-158">Логический</span><span class="sxs-lookup"><span data-stu-id="fcd5a-158">Boolean</span></span>|<span data-ttu-id="fcd5a-159">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fcd5a-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fcd5a-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="fcd5a-160">privacyInformationUrl</span></span>|<span data-ttu-id="fcd5a-161">Строка</span><span class="sxs-lookup"><span data-stu-id="fcd5a-161">String</span></span>|<span data-ttu-id="fcd5a-162">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="fcd5a-162">The privacy statement Url.</span></span> <span data-ttu-id="fcd5a-163">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fcd5a-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fcd5a-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="fcd5a-164">informationUrl</span></span>|<span data-ttu-id="fcd5a-165">Строка</span><span class="sxs-lookup"><span data-stu-id="fcd5a-165">String</span></span>|<span data-ttu-id="fcd5a-166">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="fcd5a-166">The more information Url.</span></span> <span data-ttu-id="fcd5a-167">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fcd5a-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fcd5a-168">owner</span><span class="sxs-lookup"><span data-stu-id="fcd5a-168">owner</span></span>|<span data-ttu-id="fcd5a-169">Строка</span><span class="sxs-lookup"><span data-stu-id="fcd5a-169">String</span></span>|<span data-ttu-id="fcd5a-170">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="fcd5a-170">The owner of the app.</span></span> <span data-ttu-id="fcd5a-171">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fcd5a-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fcd5a-172">developer</span><span class="sxs-lookup"><span data-stu-id="fcd5a-172">developer</span></span>|<span data-ttu-id="fcd5a-173">Строка</span><span class="sxs-lookup"><span data-stu-id="fcd5a-173">String</span></span>|<span data-ttu-id="fcd5a-174">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="fcd5a-174">The developer of the app.</span></span> <span data-ttu-id="fcd5a-175">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fcd5a-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fcd5a-176">notes</span><span class="sxs-lookup"><span data-stu-id="fcd5a-176">notes</span></span>|<span data-ttu-id="fcd5a-177">Строка</span><span class="sxs-lookup"><span data-stu-id="fcd5a-177">String</span></span>|<span data-ttu-id="fcd5a-178">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="fcd5a-178">Notes for the app.</span></span> <span data-ttu-id="fcd5a-179">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fcd5a-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fcd5a-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="fcd5a-180">publishingState</span></span>|[<span data-ttu-id="fcd5a-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="fcd5a-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="fcd5a-182">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="fcd5a-182">The publishing state for the app.</span></span> <span data-ttu-id="fcd5a-183">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="fcd5a-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="fcd5a-184">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fcd5a-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span> <span data-ttu-id="fcd5a-185">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="fcd5a-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="fcd5a-186">appAvailability</span><span class="sxs-lookup"><span data-stu-id="fcd5a-186">appAvailability</span></span>|[<span data-ttu-id="fcd5a-187">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="fcd5a-187">managedAppAvailability</span></span>](../resources/intune_apps_managedappavailability.md)|<span data-ttu-id="fcd5a-188">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="fcd5a-188">The Application's availability.</span></span> <span data-ttu-id="fcd5a-189">Наследуется от [managedApp](../resources/intune_apps_managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="fcd5a-189">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span> <span data-ttu-id="fcd5a-190">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="fcd5a-190">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="fcd5a-191">version</span><span class="sxs-lookup"><span data-stu-id="fcd5a-191">version</span></span>|<span data-ttu-id="fcd5a-192">Строка</span><span class="sxs-lookup"><span data-stu-id="fcd5a-192">String</span></span>|<span data-ttu-id="fcd5a-193">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="fcd5a-193">The Application's version.</span></span> <span data-ttu-id="fcd5a-194">Наследуется от объекта [managedApp](../resources/intune_apps_managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="fcd5a-194">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="fcd5a-195">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="fcd5a-195">committedContentVersion</span></span>|<span data-ttu-id="fcd5a-196">Строка</span><span class="sxs-lookup"><span data-stu-id="fcd5a-196">String</span></span>|<span data-ttu-id="fcd5a-197">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="fcd5a-197">The internal committed content version.</span></span> <span data-ttu-id="fcd5a-198">Наследуется от объекта [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="fcd5a-198">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="fcd5a-199">fileName</span><span class="sxs-lookup"><span data-stu-id="fcd5a-199">fileName</span></span>|<span data-ttu-id="fcd5a-200">Строка</span><span class="sxs-lookup"><span data-stu-id="fcd5a-200">String</span></span>|<span data-ttu-id="fcd5a-201">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="fcd5a-201">The name of the main Lob application file.</span></span> <span data-ttu-id="fcd5a-202">Наследуется от объекта [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="fcd5a-202">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="fcd5a-203">size</span><span class="sxs-lookup"><span data-stu-id="fcd5a-203">size</span></span>|<span data-ttu-id="fcd5a-204">Int64</span><span class="sxs-lookup"><span data-stu-id="fcd5a-204">Int64</span></span>|<span data-ttu-id="fcd5a-205">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="fcd5a-205">The total size, including all uploaded files.</span></span> <span data-ttu-id="fcd5a-206">Наследуется от объекта [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="fcd5a-206">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="fcd5a-207">bundleId</span><span class="sxs-lookup"><span data-stu-id="fcd5a-207">bundleId</span></span>|<span data-ttu-id="fcd5a-208">Строка</span><span class="sxs-lookup"><span data-stu-id="fcd5a-208">String</span></span>|<span data-ttu-id="fcd5a-209">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="fcd5a-209">The Identity Name.</span></span>|
|<span data-ttu-id="fcd5a-210">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="fcd5a-210">applicableDeviceType</span></span>|[<span data-ttu-id="fcd5a-211">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="fcd5a-211">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="fcd5a-212">Архитектура iOS, поддерживаемая этим приложением.</span><span class="sxs-lookup"><span data-stu-id="fcd5a-212">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="fcd5a-213">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="fcd5a-213">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="fcd5a-214">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="fcd5a-214">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="fcd5a-215">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="fcd5a-215">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="fcd5a-216">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="fcd5a-216">expirationDateTime</span></span>|<span data-ttu-id="fcd5a-217">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fcd5a-217">DateTimeOffset</span></span>|<span data-ttu-id="fcd5a-218">Время окончания срока действия.</span><span class="sxs-lookup"><span data-stu-id="fcd5a-218">The expiration time.</span></span>|
|<span data-ttu-id="fcd5a-219">versionNumber</span><span class="sxs-lookup"><span data-stu-id="fcd5a-219">versionNumber</span></span>|<span data-ttu-id="fcd5a-220">Строка</span><span class="sxs-lookup"><span data-stu-id="fcd5a-220">String</span></span>|<span data-ttu-id="fcd5a-221">Номер версии управляемого бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="fcd5a-221">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="fcd5a-222">buildNumber</span><span class="sxs-lookup"><span data-stu-id="fcd5a-222">buildNumber</span></span>|<span data-ttu-id="fcd5a-223">Строка</span><span class="sxs-lookup"><span data-stu-id="fcd5a-223">String</span></span>|<span data-ttu-id="fcd5a-224">Номер сборки управляемого бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="fcd5a-224">The build number of managed iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="fcd5a-225">Ответ</span><span class="sxs-lookup"><span data-stu-id="fcd5a-225">Response</span></span>
<span data-ttu-id="fcd5a-226">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="fcd5a-226">If successful, this method returns a `201 Created` response code and a [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fcd5a-227">Пример</span><span class="sxs-lookup"><span data-stu-id="fcd5a-227">Example</span></span>
### <a name="request"></a><span data-ttu-id="fcd5a-228">Запрос</span><span class="sxs-lookup"><span data-stu-id="fcd5a-228">Request</span></span>
<span data-ttu-id="fcd5a-229">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fcd5a-229">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fcd5a-230">Ответ</span><span class="sxs-lookup"><span data-stu-id="fcd5a-230">Response</span></span>
<span data-ttu-id="fcd5a-p120">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fcd5a-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








