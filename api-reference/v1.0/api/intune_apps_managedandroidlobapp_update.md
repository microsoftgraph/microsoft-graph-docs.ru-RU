# <a name="update-managedandroidlobapp"></a><span data-ttu-id="af5c6-101">Обновление managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="af5c6-101">Update managedAndroidLobApp</span></span>

> <span data-ttu-id="af5c6-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="af5c6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="af5c6-103">Обновление свойств объекта [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="af5c6-103">Update the properties of a [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="af5c6-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="af5c6-104">Prerequisites</span></span>
<span data-ttu-id="af5c6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="af5c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="af5c6-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="af5c6-107">Permission type</span></span>|<span data-ttu-id="af5c6-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="af5c6-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af5c6-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="af5c6-109">Delegated (work or school account)</span></span>|<span data-ttu-id="af5c6-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af5c6-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="af5c6-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="af5c6-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af5c6-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af5c6-112">Not supported.</span></span>|
|<span data-ttu-id="af5c6-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="af5c6-113">Application</span></span>|<span data-ttu-id="af5c6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af5c6-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="af5c6-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="af5c6-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="af5c6-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="af5c6-116">Request headers</span></span>
|<span data-ttu-id="af5c6-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="af5c6-117">Header</span></span>|<span data-ttu-id="af5c6-118">Значение</span><span class="sxs-lookup"><span data-stu-id="af5c6-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af5c6-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="af5c6-119">Authorization</span></span>|<span data-ttu-id="af5c6-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="af5c6-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af5c6-121">Принять</span><span class="sxs-lookup"><span data-stu-id="af5c6-121">Accept</span></span>|<span data-ttu-id="af5c6-122">приложение/json</span><span class="sxs-lookup"><span data-stu-id="af5c6-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af5c6-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="af5c6-123">Request body</span></span>
<span data-ttu-id="af5c6-124">В теле запроса добавьте представление объекта [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="af5c6-124">In the request body, supply a JSON representation for the [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md) object.</span></span>

<span data-ttu-id="af5c6-125">Ниже показаны свойства, которые необходимо указывать при создании объекта [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="af5c6-125">The following table shows the properties that are required when you create the [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md).</span></span>

|<span data-ttu-id="af5c6-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="af5c6-126">Property</span></span>|<span data-ttu-id="af5c6-127">Тип</span><span class="sxs-lookup"><span data-stu-id="af5c6-127">Type</span></span>|<span data-ttu-id="af5c6-128">Описание</span><span class="sxs-lookup"><span data-stu-id="af5c6-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af5c6-129">ИД</span><span class="sxs-lookup"><span data-stu-id="af5c6-129">id</span></span>|<span data-ttu-id="af5c6-130">Строка</span><span class="sxs-lookup"><span data-stu-id="af5c6-130">String</span></span>|<span data-ttu-id="af5c6-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="af5c6-131">Key of the entity.</span></span> <span data-ttu-id="af5c6-132">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af5c6-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="af5c6-133">displayName</span><span class="sxs-lookup"><span data-stu-id="af5c6-133">displayName</span></span>|<span data-ttu-id="af5c6-134">Строка</span><span class="sxs-lookup"><span data-stu-id="af5c6-134">String</span></span>|<span data-ttu-id="af5c6-135">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="af5c6-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="af5c6-136">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af5c6-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="af5c6-137">описание</span><span class="sxs-lookup"><span data-stu-id="af5c6-137">description</span></span>|<span data-ttu-id="af5c6-138">Строка</span><span class="sxs-lookup"><span data-stu-id="af5c6-138">String</span></span>|<span data-ttu-id="af5c6-139">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="af5c6-139">The description of the app.</span></span> <span data-ttu-id="af5c6-140">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af5c6-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="af5c6-141">publisher</span><span class="sxs-lookup"><span data-stu-id="af5c6-141">publisher</span></span>|<span data-ttu-id="af5c6-142">Строка</span><span class="sxs-lookup"><span data-stu-id="af5c6-142">String</span></span>|<span data-ttu-id="af5c6-143">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="af5c6-143">The publisher of the app.</span></span> <span data-ttu-id="af5c6-144">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af5c6-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="af5c6-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="af5c6-145">largeIcon</span></span>|[<span data-ttu-id="af5c6-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="af5c6-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="af5c6-147">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="af5c6-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="af5c6-148">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af5c6-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="af5c6-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="af5c6-149">createdDateTime</span></span>|<span data-ttu-id="af5c6-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af5c6-150">DateTimeOffset</span></span>|<span data-ttu-id="af5c6-151">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="af5c6-151">The date and time the app was created.</span></span> <span data-ttu-id="af5c6-152">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af5c6-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="af5c6-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="af5c6-153">lastModifiedDateTime</span></span>|<span data-ttu-id="af5c6-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af5c6-154">DateTimeOffset</span></span>|<span data-ttu-id="af5c6-155">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="af5c6-155">The date and time the app was last modified.</span></span> <span data-ttu-id="af5c6-156">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af5c6-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="af5c6-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="af5c6-157">isFeatured</span></span>|<span data-ttu-id="af5c6-158">Логический</span><span class="sxs-lookup"><span data-stu-id="af5c6-158">Boolean</span></span>|<span data-ttu-id="af5c6-159">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af5c6-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="af5c6-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="af5c6-160">privacyInformationUrl</span></span>|<span data-ttu-id="af5c6-161">Строка</span><span class="sxs-lookup"><span data-stu-id="af5c6-161">String</span></span>|<span data-ttu-id="af5c6-162">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="af5c6-162">The privacy statement Url.</span></span> <span data-ttu-id="af5c6-163">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af5c6-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="af5c6-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="af5c6-164">informationUrl</span></span>|<span data-ttu-id="af5c6-165">Строка</span><span class="sxs-lookup"><span data-stu-id="af5c6-165">String</span></span>|<span data-ttu-id="af5c6-166">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="af5c6-166">The more information Url.</span></span> <span data-ttu-id="af5c6-167">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af5c6-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="af5c6-168">владелец</span><span class="sxs-lookup"><span data-stu-id="af5c6-168">owner</span></span>|<span data-ttu-id="af5c6-169">Строка</span><span class="sxs-lookup"><span data-stu-id="af5c6-169">String</span></span>|<span data-ttu-id="af5c6-170">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="af5c6-170">The owner of the app.</span></span> <span data-ttu-id="af5c6-171">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af5c6-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="af5c6-172">разработчик</span><span class="sxs-lookup"><span data-stu-id="af5c6-172">developer</span></span>|<span data-ttu-id="af5c6-173">Строка</span><span class="sxs-lookup"><span data-stu-id="af5c6-173">String</span></span>|<span data-ttu-id="af5c6-174">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="af5c6-174">The developer of the app.</span></span> <span data-ttu-id="af5c6-175">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af5c6-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="af5c6-176">примечания</span><span class="sxs-lookup"><span data-stu-id="af5c6-176">notes</span></span>|<span data-ttu-id="af5c6-177">Строка</span><span class="sxs-lookup"><span data-stu-id="af5c6-177">String</span></span>|<span data-ttu-id="af5c6-178">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="af5c6-178">Notes for the app.</span></span> <span data-ttu-id="af5c6-179">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af5c6-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="af5c6-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="af5c6-180">publishingState</span></span>|[<span data-ttu-id="af5c6-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="af5c6-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="af5c6-182">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="af5c6-182">The publishing state for the app.</span></span> <span data-ttu-id="af5c6-183">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="af5c6-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="af5c6-184">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af5c6-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span> <span data-ttu-id="af5c6-185">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="af5c6-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="af5c6-186">appAvailability</span><span class="sxs-lookup"><span data-stu-id="af5c6-186">appAvailability</span></span>|[<span data-ttu-id="af5c6-187">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="af5c6-187">managedAppAvailability</span></span>](../resources/intune_apps_managedappavailability.md)|<span data-ttu-id="af5c6-188">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="af5c6-188">The Application's availability.</span></span> <span data-ttu-id="af5c6-189">Наследуется от [managedApp](../resources/intune_apps_managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="af5c6-189">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span> <span data-ttu-id="af5c6-190">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="af5c6-190">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="af5c6-191">версия</span><span class="sxs-lookup"><span data-stu-id="af5c6-191">version</span></span>|<span data-ttu-id="af5c6-192">Строка</span><span class="sxs-lookup"><span data-stu-id="af5c6-192">String</span></span>|<span data-ttu-id="af5c6-193">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="af5c6-193">The Application's version.</span></span> <span data-ttu-id="af5c6-194">Наследуется от объекта [managedApp](../resources/intune_apps_managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="af5c6-194">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="af5c6-195">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="af5c6-195">committedContentVersion</span></span>|<span data-ttu-id="af5c6-196">Строка</span><span class="sxs-lookup"><span data-stu-id="af5c6-196">String</span></span>|<span data-ttu-id="af5c6-197">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="af5c6-197">The internal committed content version.</span></span> <span data-ttu-id="af5c6-198">Наследуется от объекта [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="af5c6-198">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="af5c6-199">fileName</span><span class="sxs-lookup"><span data-stu-id="af5c6-199">fileName</span></span>|<span data-ttu-id="af5c6-200">Строка</span><span class="sxs-lookup"><span data-stu-id="af5c6-200">String</span></span>|<span data-ttu-id="af5c6-201">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="af5c6-201">The name of the main Lob application file.</span></span> <span data-ttu-id="af5c6-202">Наследуется от объекта [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="af5c6-202">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="af5c6-203">изменить размер</span><span class="sxs-lookup"><span data-stu-id="af5c6-203">size</span></span>|<span data-ttu-id="af5c6-204">Int64</span><span class="sxs-lookup"><span data-stu-id="af5c6-204">Int64</span></span>|<span data-ttu-id="af5c6-205">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="af5c6-205">The total size, including all uploaded files.</span></span> <span data-ttu-id="af5c6-206">Наследуется от объекта [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="af5c6-206">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="af5c6-207">packageId</span><span class="sxs-lookup"><span data-stu-id="af5c6-207">packageId</span></span>|<span data-ttu-id="af5c6-208">Строка</span><span class="sxs-lookup"><span data-stu-id="af5c6-208">String</span></span>|<span data-ttu-id="af5c6-209">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="af5c6-209">The package identifier.</span></span>|
|<span data-ttu-id="af5c6-210">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="af5c6-210">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="af5c6-211">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="af5c6-211">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="af5c6-212">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="af5c6-212">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="af5c6-213">versionName</span><span class="sxs-lookup"><span data-stu-id="af5c6-213">versionName</span></span>|<span data-ttu-id="af5c6-214">Строка</span><span class="sxs-lookup"><span data-stu-id="af5c6-214">String</span></span>|<span data-ttu-id="af5c6-215">Имя версии управляемого бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="af5c6-215">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="af5c6-216">versionCode</span><span class="sxs-lookup"><span data-stu-id="af5c6-216">versionCode</span></span>|<span data-ttu-id="af5c6-217">Строка</span><span class="sxs-lookup"><span data-stu-id="af5c6-217">String</span></span>|<span data-ttu-id="af5c6-218">Код версии управляемого бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="af5c6-218">The version code of managed Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="af5c6-219">Ответ</span><span class="sxs-lookup"><span data-stu-id="af5c6-219">Response</span></span>
<span data-ttu-id="af5c6-220">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="af5c6-220">If successful, this method returns a `200 OK` response code and an updated [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af5c6-221">Пример</span><span class="sxs-lookup"><span data-stu-id="af5c6-221">Example</span></span>
### <a name="request"></a><span data-ttu-id="af5c6-222">Запрос</span><span class="sxs-lookup"><span data-stu-id="af5c6-222">Request</span></span>
<span data-ttu-id="af5c6-223">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="af5c6-223">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1158

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

### <a name="response"></a><span data-ttu-id="af5c6-224">Ответ</span><span class="sxs-lookup"><span data-stu-id="af5c6-224">Response</span></span>
<span data-ttu-id="af5c6-p120">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="af5c6-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1325

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
  "id": "802b7ed3-7ed3-802b-d37e-2b80d37e2b80",
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








