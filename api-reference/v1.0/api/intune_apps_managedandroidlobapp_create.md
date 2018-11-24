# <a name="create-managedandroidlobapp"></a><span data-ttu-id="95b27-101">Create managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="95b27-101">Create managedAndroidLobApp</span></span>

> <span data-ttu-id="95b27-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="95b27-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="95b27-103">Создание объекта [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="95b27-103">Create a new [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="95b27-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="95b27-104">Prerequisites</span></span>
<span data-ttu-id="95b27-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="95b27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="95b27-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="95b27-107">Permission type</span></span>|<span data-ttu-id="95b27-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="95b27-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95b27-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="95b27-109">Delegated (work or school account)</span></span>|<span data-ttu-id="95b27-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95b27-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="95b27-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="95b27-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95b27-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95b27-112">Not supported.</span></span>|
|<span data-ttu-id="95b27-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="95b27-113">Application</span></span>|<span data-ttu-id="95b27-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95b27-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="95b27-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="95b27-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="95b27-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="95b27-116">Request headers</span></span>
|<span data-ttu-id="95b27-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="95b27-117">Header</span></span>|<span data-ttu-id="95b27-118">Значение</span><span class="sxs-lookup"><span data-stu-id="95b27-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95b27-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="95b27-119">Authorization</span></span>|<span data-ttu-id="95b27-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="95b27-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95b27-121">Accept</span><span class="sxs-lookup"><span data-stu-id="95b27-121">Accept</span></span>|<span data-ttu-id="95b27-122">application/json</span><span class="sxs-lookup"><span data-stu-id="95b27-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95b27-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="95b27-123">Request body</span></span>
<span data-ttu-id="95b27-124">В тексте запроса добавьте представление объекта managedAndroidLobApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="95b27-124">In the request body, supply a JSON representation for the managedAndroidLobApp object.</span></span>

<span data-ttu-id="95b27-125">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта managedAndroidLobApp.</span><span class="sxs-lookup"><span data-stu-id="95b27-125">The following table shows the properties that are required when you create the managedAndroidLobApp.</span></span>

|<span data-ttu-id="95b27-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="95b27-126">Property</span></span>|<span data-ttu-id="95b27-127">Тип</span><span class="sxs-lookup"><span data-stu-id="95b27-127">Type</span></span>|<span data-ttu-id="95b27-128">Описание</span><span class="sxs-lookup"><span data-stu-id="95b27-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95b27-129">id</span><span class="sxs-lookup"><span data-stu-id="95b27-129">id</span></span>|<span data-ttu-id="95b27-130">String</span><span class="sxs-lookup"><span data-stu-id="95b27-130">String</span></span>|<span data-ttu-id="95b27-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="95b27-131">Key of the entity.</span></span> <span data-ttu-id="95b27-132">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95b27-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="95b27-133">displayName</span><span class="sxs-lookup"><span data-stu-id="95b27-133">displayName</span></span>|<span data-ttu-id="95b27-134">String</span><span class="sxs-lookup"><span data-stu-id="95b27-134">String</span></span>|<span data-ttu-id="95b27-135">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="95b27-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="95b27-136">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95b27-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="95b27-137">description</span><span class="sxs-lookup"><span data-stu-id="95b27-137">description</span></span>|<span data-ttu-id="95b27-138">String</span><span class="sxs-lookup"><span data-stu-id="95b27-138">String</span></span>|<span data-ttu-id="95b27-139">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="95b27-139">The description of the app.</span></span> <span data-ttu-id="95b27-140">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95b27-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="95b27-141">publisher</span><span class="sxs-lookup"><span data-stu-id="95b27-141">publisher</span></span>|<span data-ttu-id="95b27-142">String</span><span class="sxs-lookup"><span data-stu-id="95b27-142">String</span></span>|<span data-ttu-id="95b27-143">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="95b27-143">The publisher of the app.</span></span> <span data-ttu-id="95b27-144">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95b27-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="95b27-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="95b27-145">largeIcon</span></span>|[<span data-ttu-id="95b27-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="95b27-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="95b27-147">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="95b27-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="95b27-148">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95b27-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="95b27-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="95b27-149">createdDateTime</span></span>|<span data-ttu-id="95b27-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95b27-150">DateTimeOffset</span></span>|<span data-ttu-id="95b27-151">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="95b27-151">The date and time the app was created.</span></span> <span data-ttu-id="95b27-152">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95b27-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="95b27-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="95b27-153">lastModifiedDateTime</span></span>|<span data-ttu-id="95b27-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95b27-154">DateTimeOffset</span></span>|<span data-ttu-id="95b27-155">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="95b27-155">The date and time the app was last modified.</span></span> <span data-ttu-id="95b27-156">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95b27-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="95b27-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="95b27-157">isFeatured</span></span>|<span data-ttu-id="95b27-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="95b27-158">Boolean</span></span>|<span data-ttu-id="95b27-159">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95b27-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="95b27-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="95b27-160">privacyInformationUrl</span></span>|<span data-ttu-id="95b27-161">String</span><span class="sxs-lookup"><span data-stu-id="95b27-161">String</span></span>|<span data-ttu-id="95b27-162">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="95b27-162">The privacy statement Url.</span></span> <span data-ttu-id="95b27-163">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95b27-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="95b27-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="95b27-164">informationUrl</span></span>|<span data-ttu-id="95b27-165">String</span><span class="sxs-lookup"><span data-stu-id="95b27-165">String</span></span>|<span data-ttu-id="95b27-166">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="95b27-166">The more information Url.</span></span> <span data-ttu-id="95b27-167">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95b27-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="95b27-168">owner</span><span class="sxs-lookup"><span data-stu-id="95b27-168">owner</span></span>|<span data-ttu-id="95b27-169">String</span><span class="sxs-lookup"><span data-stu-id="95b27-169">String</span></span>|<span data-ttu-id="95b27-170">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="95b27-170">The owner of the app.</span></span> <span data-ttu-id="95b27-171">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95b27-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="95b27-172">developer</span><span class="sxs-lookup"><span data-stu-id="95b27-172">developer</span></span>|<span data-ttu-id="95b27-173">String</span><span class="sxs-lookup"><span data-stu-id="95b27-173">String</span></span>|<span data-ttu-id="95b27-174">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="95b27-174">The developer of the app.</span></span> <span data-ttu-id="95b27-175">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95b27-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="95b27-176">notes</span><span class="sxs-lookup"><span data-stu-id="95b27-176">notes</span></span>|<span data-ttu-id="95b27-177">String</span><span class="sxs-lookup"><span data-stu-id="95b27-177">String</span></span>|<span data-ttu-id="95b27-178">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="95b27-178">Notes for the app.</span></span> <span data-ttu-id="95b27-179">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95b27-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="95b27-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="95b27-180">publishingState</span></span>|[<span data-ttu-id="95b27-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="95b27-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="95b27-182">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="95b27-182">The publishing state for the app.</span></span> <span data-ttu-id="95b27-183">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="95b27-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="95b27-184">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95b27-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md).</span></span> <span data-ttu-id="95b27-185">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="95b27-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="95b27-186">appAvailability</span><span class="sxs-lookup"><span data-stu-id="95b27-186">appAvailability</span></span>|[<span data-ttu-id="95b27-187">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="95b27-187">managedAppAvailability</span></span>](../resources/intune_apps_managedappavailability.md)|<span data-ttu-id="95b27-188">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="95b27-188">The Application's availability.</span></span> <span data-ttu-id="95b27-189">Наследуется от [managedApp](../resources/intune_apps_managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="95b27-189">Inherited from [managedApp](../resources/intune_apps_managedapp.md).</span></span> <span data-ttu-id="95b27-190">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="95b27-190">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="95b27-191">version</span><span class="sxs-lookup"><span data-stu-id="95b27-191">version</span></span>|<span data-ttu-id="95b27-192">String</span><span class="sxs-lookup"><span data-stu-id="95b27-192">String</span></span>|<span data-ttu-id="95b27-193">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="95b27-193">The Application's version.</span></span> <span data-ttu-id="95b27-194">Наследуется от объекта [managedApp](../resources/intune_apps_managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="95b27-194">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="95b27-195">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="95b27-195">committedContentVersion</span></span>|<span data-ttu-id="95b27-196">String</span><span class="sxs-lookup"><span data-stu-id="95b27-196">String</span></span>|<span data-ttu-id="95b27-197">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="95b27-197">The internal committed content version.</span></span> <span data-ttu-id="95b27-198">Наследуется от объекта [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="95b27-198">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="95b27-199">fileName</span><span class="sxs-lookup"><span data-stu-id="95b27-199">fileName</span></span>|<span data-ttu-id="95b27-200">String</span><span class="sxs-lookup"><span data-stu-id="95b27-200">String</span></span>|<span data-ttu-id="95b27-201">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="95b27-201">The name of the main Lob application file.</span></span> <span data-ttu-id="95b27-202">Наследуется от объекта [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="95b27-202">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="95b27-203">size</span><span class="sxs-lookup"><span data-stu-id="95b27-203">size</span></span>|<span data-ttu-id="95b27-204">Int64</span><span class="sxs-lookup"><span data-stu-id="95b27-204">Int64</span></span>|<span data-ttu-id="95b27-205">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="95b27-205">The total size, including all uploaded files.</span></span> <span data-ttu-id="95b27-206">Наследуется от объекта [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="95b27-206">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="95b27-207">packageId</span><span class="sxs-lookup"><span data-stu-id="95b27-207">packageId</span></span>|<span data-ttu-id="95b27-208">String</span><span class="sxs-lookup"><span data-stu-id="95b27-208">String</span></span>|<span data-ttu-id="95b27-209">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="95b27-209">The package identifier.</span></span>|
|<span data-ttu-id="95b27-210">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="95b27-210">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="95b27-211">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="95b27-211">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="95b27-212">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="95b27-212">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="95b27-213">versionName</span><span class="sxs-lookup"><span data-stu-id="95b27-213">versionName</span></span>|<span data-ttu-id="95b27-214">String</span><span class="sxs-lookup"><span data-stu-id="95b27-214">String</span></span>|<span data-ttu-id="95b27-215">Имя версии управляемого бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="95b27-215">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="95b27-216">versionCode</span><span class="sxs-lookup"><span data-stu-id="95b27-216">versionCode</span></span>|<span data-ttu-id="95b27-217">String</span><span class="sxs-lookup"><span data-stu-id="95b27-217">String</span></span>|<span data-ttu-id="95b27-218">Код версии управляемого бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="95b27-218">The version code of managed Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="95b27-219">Ответ</span><span class="sxs-lookup"><span data-stu-id="95b27-219">Response</span></span>
<span data-ttu-id="95b27-220">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="95b27-220">If successful, this method returns a `201 Created` response code and a [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95b27-221">Пример</span><span class="sxs-lookup"><span data-stu-id="95b27-221">Example</span></span>
### <a name="request"></a><span data-ttu-id="95b27-222">Запрос</span><span class="sxs-lookup"><span data-stu-id="95b27-222">Request</span></span>
<span data-ttu-id="95b27-223">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="95b27-223">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1153

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
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

### <a name="response"></a><span data-ttu-id="95b27-224">Ответ</span><span class="sxs-lookup"><span data-stu-id="95b27-224">Response</span></span>
<span data-ttu-id="95b27-p120">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="95b27-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



