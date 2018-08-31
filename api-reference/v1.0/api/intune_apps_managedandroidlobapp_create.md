# <a name="create-managedandroidlobapp"></a><span data-ttu-id="b8be9-101">Создание managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="b8be9-101">Create managedAndroidLobApp</span></span>

> <span data-ttu-id="b8be9-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b8be9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b8be9-103">Создание объекта [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="b8be9-103">Create a new [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b8be9-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="b8be9-104">Prerequisites</span></span>
<span data-ttu-id="b8be9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b8be9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b8be9-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b8be9-107">Permission type</span></span>|<span data-ttu-id="b8be9-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b8be9-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8be9-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b8be9-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b8be9-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8be9-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b8be9-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b8be9-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8be9-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8be9-112">Not supported.</span></span>|
|<span data-ttu-id="b8be9-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b8be9-113">Application</span></span>|<span data-ttu-id="b8be9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8be9-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8be9-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b8be9-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="b8be9-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b8be9-116">Request headers</span></span>
|<span data-ttu-id="b8be9-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b8be9-117">Header</span></span>|<span data-ttu-id="b8be9-118">Значение</span><span class="sxs-lookup"><span data-stu-id="b8be9-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8be9-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b8be9-119">Authorization</span></span>|<span data-ttu-id="b8be9-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="b8be9-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8be9-121">Accept</span><span class="sxs-lookup"><span data-stu-id="b8be9-121">Accept</span></span>|<span data-ttu-id="b8be9-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b8be9-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8be9-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b8be9-123">Request body</span></span>
<span data-ttu-id="b8be9-124">В тексте запроса добавьте представление объекта managedAndroidLobApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b8be9-124">In the request body, supply a JSON representation for the managedAndroidLobApp object.</span></span>

<span data-ttu-id="b8be9-125">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта managedAndroidLobApp.</span><span class="sxs-lookup"><span data-stu-id="b8be9-125">The following table shows the properties that are required when you create the managedAndroidLobApp.</span></span>

|<span data-ttu-id="b8be9-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="b8be9-126">Property</span></span>|<span data-ttu-id="b8be9-127">Тип</span><span class="sxs-lookup"><span data-stu-id="b8be9-127">Type</span></span>|<span data-ttu-id="b8be9-128">Описание</span><span class="sxs-lookup"><span data-stu-id="b8be9-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8be9-129">id</span><span class="sxs-lookup"><span data-stu-id="b8be9-129">id</span></span>|<span data-ttu-id="b8be9-130">String (строка)</span><span class="sxs-lookup"><span data-stu-id="b8be9-130">String</span></span>|<span data-ttu-id="b8be9-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b8be9-131">Key of the entity.</span></span> <span data-ttu-id="b8be9-132">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b8be9-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b8be9-133">displayName</span><span class="sxs-lookup"><span data-stu-id="b8be9-133">displayName</span></span>|<span data-ttu-id="b8be9-134">String (строка)</span><span class="sxs-lookup"><span data-stu-id="b8be9-134">String</span></span>|<span data-ttu-id="b8be9-135">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="b8be9-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b8be9-136">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b8be9-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b8be9-137">description</span><span class="sxs-lookup"><span data-stu-id="b8be9-137">description</span></span>|<span data-ttu-id="b8be9-138">String (строка)</span><span class="sxs-lookup"><span data-stu-id="b8be9-138">String</span></span>|<span data-ttu-id="b8be9-139">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="b8be9-139">The description of the app.</span></span> <span data-ttu-id="b8be9-140">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b8be9-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b8be9-141">publisher</span><span class="sxs-lookup"><span data-stu-id="b8be9-141">publisher</span></span>|<span data-ttu-id="b8be9-142">String (строка)</span><span class="sxs-lookup"><span data-stu-id="b8be9-142">String</span></span>|<span data-ttu-id="b8be9-143">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="b8be9-143">The publisher of the app.</span></span> <span data-ttu-id="b8be9-144">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b8be9-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b8be9-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b8be9-145">largeIcon</span></span>|[<span data-ttu-id="b8be9-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b8be9-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="b8be9-147">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="b8be9-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b8be9-148">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b8be9-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b8be9-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b8be9-149">createdDateTime</span></span>|<span data-ttu-id="b8be9-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8be9-150">DateTimeOffset</span></span>|<span data-ttu-id="b8be9-151">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="b8be9-151">The date and time the app was created.</span></span> <span data-ttu-id="b8be9-152">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b8be9-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b8be9-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b8be9-153">lastModifiedDateTime</span></span>|<span data-ttu-id="b8be9-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8be9-154">DateTimeOffset</span></span>|<span data-ttu-id="b8be9-155">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="b8be9-155">The date and time the app was last modified.</span></span> <span data-ttu-id="b8be9-156">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b8be9-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b8be9-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b8be9-157">isFeatured</span></span>|<span data-ttu-id="b8be9-158">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="b8be9-158">Boolean</span></span>|<span data-ttu-id="b8be9-159">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b8be9-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b8be9-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b8be9-160">privacyInformationUrl</span></span>|<span data-ttu-id="b8be9-161">String (строка)</span><span class="sxs-lookup"><span data-stu-id="b8be9-161">String</span></span>|<span data-ttu-id="b8be9-162">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="b8be9-162">The privacy statement Url.</span></span> <span data-ttu-id="b8be9-163">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b8be9-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b8be9-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b8be9-164">informationUrl</span></span>|<span data-ttu-id="b8be9-165">String (строка)</span><span class="sxs-lookup"><span data-stu-id="b8be9-165">String</span></span>|<span data-ttu-id="b8be9-166">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="b8be9-166">The more information Url.</span></span> <span data-ttu-id="b8be9-167">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b8be9-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b8be9-168">owner</span><span class="sxs-lookup"><span data-stu-id="b8be9-168">owner</span></span>|<span data-ttu-id="b8be9-169">String (строка)</span><span class="sxs-lookup"><span data-stu-id="b8be9-169">String</span></span>|<span data-ttu-id="b8be9-170">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="b8be9-170">The owner of the app.</span></span> <span data-ttu-id="b8be9-171">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b8be9-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b8be9-172">developer</span><span class="sxs-lookup"><span data-stu-id="b8be9-172">developer</span></span>|<span data-ttu-id="b8be9-173">String (строка)</span><span class="sxs-lookup"><span data-stu-id="b8be9-173">String</span></span>|<span data-ttu-id="b8be9-174">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="b8be9-174">The developer of the app.</span></span> <span data-ttu-id="b8be9-175">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b8be9-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b8be9-176">notes</span><span class="sxs-lookup"><span data-stu-id="b8be9-176">notes</span></span>|<span data-ttu-id="b8be9-177">String (строка)</span><span class="sxs-lookup"><span data-stu-id="b8be9-177">String</span></span>|<span data-ttu-id="b8be9-178">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="b8be9-178">Notes for the app.</span></span> <span data-ttu-id="b8be9-179">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b8be9-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b8be9-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="b8be9-180">publishingState</span></span>|[<span data-ttu-id="b8be9-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="b8be9-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="b8be9-182">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="b8be9-182">The publishing state for the app.</span></span> <span data-ttu-id="b8be9-183">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="b8be9-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b8be9-184">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b8be9-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span> <span data-ttu-id="b8be9-185">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="b8be9-185">The possible values are `notPublished`, `processing`, `published`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="b8be9-186">appAvailability</span><span class="sxs-lookup"><span data-stu-id="b8be9-186">appAvailability</span></span>|[<span data-ttu-id="b8be9-187">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="b8be9-187">managedAppAvailability</span></span>](../resources/intune_apps_managedappavailability.md)|<span data-ttu-id="b8be9-188">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="b8be9-188">The Application's availability.</span></span> <span data-ttu-id="b8be9-189">Наследуется от объекта [managedApp](../resources/intune_apps_managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="b8be9-189">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span> <span data-ttu-id="b8be9-190">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="b8be9-190">The possible values are:</span></span>|
|<span data-ttu-id="b8be9-191">version</span><span class="sxs-lookup"><span data-stu-id="b8be9-191">version</span></span>|<span data-ttu-id="b8be9-192">String (строка)</span><span class="sxs-lookup"><span data-stu-id="b8be9-192">String</span></span>|<span data-ttu-id="b8be9-193">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="b8be9-193">The Application's version.</span></span> <span data-ttu-id="b8be9-194">Наследуется от объекта [managedApp](../resources/intune_apps_managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="b8be9-194">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="b8be9-195">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="b8be9-195">committedContentVersion</span></span>|<span data-ttu-id="b8be9-196">String (строка)</span><span class="sxs-lookup"><span data-stu-id="b8be9-196">String</span></span>|<span data-ttu-id="b8be9-197">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="b8be9-197">The internal committed content version.</span></span> <span data-ttu-id="b8be9-198">Наследуется от объекта [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="b8be9-198">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="b8be9-199">fileName</span><span class="sxs-lookup"><span data-stu-id="b8be9-199">fileName</span></span>|<span data-ttu-id="b8be9-200">String (строка)</span><span class="sxs-lookup"><span data-stu-id="b8be9-200">String</span></span>|<span data-ttu-id="b8be9-201">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="b8be9-201">The name of the main Lob application file.</span></span> <span data-ttu-id="b8be9-202">Наследуется от объекта [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="b8be9-202">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="b8be9-203">size</span><span class="sxs-lookup"><span data-stu-id="b8be9-203">size</span></span>|<span data-ttu-id="b8be9-204">Int64</span><span class="sxs-lookup"><span data-stu-id="b8be9-204">Int64</span></span>|<span data-ttu-id="b8be9-205">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="b8be9-205">The total size, including all uploaded files.</span></span> <span data-ttu-id="b8be9-206">Наследуется от объекта [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="b8be9-206">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="b8be9-207">packageId</span><span class="sxs-lookup"><span data-stu-id="b8be9-207">packageId</span></span>|<span data-ttu-id="b8be9-208">String (строка)</span><span class="sxs-lookup"><span data-stu-id="b8be9-208">String</span></span>|<span data-ttu-id="b8be9-209">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="b8be9-209">The package identifier.</span></span>|
|<span data-ttu-id="b8be9-210">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b8be9-210">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="b8be9-211">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b8be9-211">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="b8be9-212">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="b8be9-212">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="b8be9-213">versionName</span><span class="sxs-lookup"><span data-stu-id="b8be9-213">versionName</span></span>|<span data-ttu-id="b8be9-214">String (строка)</span><span class="sxs-lookup"><span data-stu-id="b8be9-214">String</span></span>|<span data-ttu-id="b8be9-215">Имя версии управляемого бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="b8be9-215">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="b8be9-216">versionCode</span><span class="sxs-lookup"><span data-stu-id="b8be9-216">versionCode</span></span>|<span data-ttu-id="b8be9-217">String (строка)</span><span class="sxs-lookup"><span data-stu-id="b8be9-217">String</span></span>|<span data-ttu-id="b8be9-218">Код версии управляемого бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="b8be9-218">The version code of managed Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="b8be9-219">Ответ</span><span class="sxs-lookup"><span data-stu-id="b8be9-219">Response</span></span>
<span data-ttu-id="b8be9-220">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b8be9-220">If successful, this method returns a `201 Created` response code and a [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8be9-221">Пример</span><span class="sxs-lookup"><span data-stu-id="b8be9-221">Example</span></span>
### <a name="request"></a><span data-ttu-id="b8be9-222">Запрос</span><span class="sxs-lookup"><span data-stu-id="b8be9-222">Request</span></span>
<span data-ttu-id="b8be9-223">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b8be9-223">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1217

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

### <a name="response"></a><span data-ttu-id="b8be9-224">Ответ</span><span class="sxs-lookup"><span data-stu-id="b8be9-224">Response</span></span>
<span data-ttu-id="b8be9-p120">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b8be9-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



