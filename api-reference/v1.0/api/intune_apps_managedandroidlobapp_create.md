# <a name="create-managedandroidlobapp"></a><span data-ttu-id="4b8f4-101">Create managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="4b8f4-101">Create managedAndroidLobApp</span></span>

> <span data-ttu-id="4b8f4-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4b8f4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4b8f4-103">Создание объекта [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="4b8f4-103">Create a new [plannerBucket](../resources/intune_apps_managedandroidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4b8f4-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="4b8f4-104">Prerequisites</span></span>
<span data-ttu-id="4b8f4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4b8f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4b8f4-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b8f4-107">Permission type</span></span>|<span data-ttu-id="4b8f4-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b8f4-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b8f4-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b8f4-109">Delegated (work or school account)</span></span>|<span data-ttu-id="4b8f4-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b8f4-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4b8f4-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b8f4-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b8f4-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b8f4-112">Not supported.</span></span>|
|<span data-ttu-id="4b8f4-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b8f4-113">Application</span></span>|<span data-ttu-id="4b8f4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b8f4-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b8f4-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b8f4-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="4b8f4-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4b8f4-116">Request headers</span></span>
|<span data-ttu-id="4b8f4-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4b8f4-117">Header</span></span>|<span data-ttu-id="4b8f4-118">Значение</span><span class="sxs-lookup"><span data-stu-id="4b8f4-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b8f4-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b8f4-119">Authorization</span></span>|<span data-ttu-id="4b8f4-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b8f4-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4b8f4-121">Accept</span><span class="sxs-lookup"><span data-stu-id="4b8f4-121">Accept</span></span>|<span data-ttu-id="4b8f4-122">application/json</span><span class="sxs-lookup"><span data-stu-id="4b8f4-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b8f4-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4b8f4-123">Request body</span></span>
<span data-ttu-id="4b8f4-124">В тексте запроса добавьте представление объекта managedAndroidLobApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4b8f4-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="4b8f4-125">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта managedAndroidLobApp.</span><span class="sxs-lookup"><span data-stu-id="4b8f4-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="4b8f4-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b8f4-126">Property</span></span>|<span data-ttu-id="4b8f4-127">Тип</span><span class="sxs-lookup"><span data-stu-id="4b8f4-127">Type</span></span>|<span data-ttu-id="4b8f4-128">Описание</span><span class="sxs-lookup"><span data-stu-id="4b8f4-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b8f4-129">id</span><span class="sxs-lookup"><span data-stu-id="4b8f4-129">id</span></span>|<span data-ttu-id="4b8f4-130">String</span><span class="sxs-lookup"><span data-stu-id="4b8f4-130">String</span></span>|<span data-ttu-id="4b8f4-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4b8f4-131">Key of the setting.</span></span> <span data-ttu-id="4b8f4-132">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4b8f4-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="4b8f4-133">displayName</span><span class="sxs-lookup"><span data-stu-id="4b8f4-133">displayName</span></span>|<span data-ttu-id="4b8f4-134">String</span><span class="sxs-lookup"><span data-stu-id="4b8f4-134">String</span></span>|<span data-ttu-id="4b8f4-135">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="4b8f4-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="4b8f4-136">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4b8f4-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="4b8f4-137">description</span><span class="sxs-lookup"><span data-stu-id="4b8f4-137">description</span></span>|<span data-ttu-id="4b8f4-138">String</span><span class="sxs-lookup"><span data-stu-id="4b8f4-138">String</span></span>|<span data-ttu-id="4b8f4-139">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="4b8f4-139">The description of the app.</span></span> <span data-ttu-id="4b8f4-140">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4b8f4-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="4b8f4-141">publisher</span><span class="sxs-lookup"><span data-stu-id="4b8f4-141">Publisher</span></span>|<span data-ttu-id="4b8f4-142">String</span><span class="sxs-lookup"><span data-stu-id="4b8f4-142">String</span></span>|<span data-ttu-id="4b8f4-143">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="4b8f4-143">The name of the app.</span></span> <span data-ttu-id="4b8f4-144">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4b8f4-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="4b8f4-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="4b8f4-145">largeIcon</span></span>|[<span data-ttu-id="4b8f4-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="4b8f4-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="4b8f4-147">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="4b8f4-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="4b8f4-148">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4b8f4-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="4b8f4-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4b8f4-149">createdDateTime</span></span>|<span data-ttu-id="4b8f4-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b8f4-150">DateTimeOffset</span></span>|<span data-ttu-id="4b8f4-151">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="4b8f4-151">The date and time the group was created.</span></span> <span data-ttu-id="4b8f4-152">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4b8f4-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="4b8f4-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4b8f4-153">lastModifiedDateTime</span></span>|<span data-ttu-id="4b8f4-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b8f4-154">DateTimeOffset</span></span>|<span data-ttu-id="4b8f4-155">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="4b8f4-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="4b8f4-156">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4b8f4-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="4b8f4-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="4b8f4-157">isFeatured</span></span>|<span data-ttu-id="4b8f4-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b8f4-158">Boolean</span></span>|<span data-ttu-id="4b8f4-159">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4b8f4-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="4b8f4-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="4b8f4-160">privacyInformationUrl</span></span>|<span data-ttu-id="4b8f4-161">String</span><span class="sxs-lookup"><span data-stu-id="4b8f4-161">String</span></span>|<span data-ttu-id="4b8f4-162">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="4b8f4-162">The privacy statement Url.</span></span> <span data-ttu-id="4b8f4-163">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4b8f4-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="4b8f4-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="4b8f4-164">informationUrl</span></span>|<span data-ttu-id="4b8f4-165">String</span><span class="sxs-lookup"><span data-stu-id="4b8f4-165">String</span></span>|<span data-ttu-id="4b8f4-166">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="4b8f4-166">The more information Url.</span></span> <span data-ttu-id="4b8f4-167">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4b8f4-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="4b8f4-168">owner</span><span class="sxs-lookup"><span data-stu-id="4b8f4-168">owner</span></span>|<span data-ttu-id="4b8f4-169">String</span><span class="sxs-lookup"><span data-stu-id="4b8f4-169">String</span></span>|<span data-ttu-id="4b8f4-170">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="4b8f4-170">The owner of the app.</span></span> <span data-ttu-id="4b8f4-171">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4b8f4-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="4b8f4-172">developer</span><span class="sxs-lookup"><span data-stu-id="4b8f4-172">developer</span></span>|<span data-ttu-id="4b8f4-173">String</span><span class="sxs-lookup"><span data-stu-id="4b8f4-173">String</span></span>|<span data-ttu-id="4b8f4-174">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="4b8f4-174">The name of the app.</span></span> <span data-ttu-id="4b8f4-175">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4b8f4-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="4b8f4-176">notes</span><span class="sxs-lookup"><span data-stu-id="4b8f4-176">Notes</span></span>|<span data-ttu-id="4b8f4-177">String</span><span class="sxs-lookup"><span data-stu-id="4b8f4-177">String</span></span>|<span data-ttu-id="4b8f4-178">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="4b8f4-178">Notes for the app.</span></span> <span data-ttu-id="4b8f4-179">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4b8f4-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="4b8f4-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="4b8f4-180">publishingState</span></span>|<span data-ttu-id="4b8f4-181">String</span><span class="sxs-lookup"><span data-stu-id="4b8f4-181">String</span></span>|<span data-ttu-id="4b8f4-182">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="4b8f4-182">The publishing state for the app.</span></span> <span data-ttu-id="4b8f4-183">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="4b8f4-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="4b8f4-184">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md). Допустимые значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="4b8f4-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="4b8f4-185">appAvailability</span><span class="sxs-lookup"><span data-stu-id="4b8f4-185">appAvailability</span></span>|<span data-ttu-id="4b8f4-186">String</span><span class="sxs-lookup"><span data-stu-id="4b8f4-186">String</span></span>|<span data-ttu-id="4b8f4-187">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="4b8f4-187">The Application's availability.</span></span> <span data-ttu-id="4b8f4-188">Наследуется от объекта [managedApp](../resources/intune_apps_managedapp.md). Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="4b8f4-188">Inherited from [managedApp](../resources/intune_apps_managedapp.md) Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="4b8f4-189">version</span><span class="sxs-lookup"><span data-stu-id="4b8f4-189">version</span></span>|<span data-ttu-id="4b8f4-190">String</span><span class="sxs-lookup"><span data-stu-id="4b8f4-190">String</span></span>|<span data-ttu-id="4b8f4-191">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="4b8f4-191">The Application's version.</span></span> <span data-ttu-id="4b8f4-192">Наследуется от объекта [managedApp](../resources/intune_apps_managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="4b8f4-192">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="4b8f4-193">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="4b8f4-193">committedContentVersion</span></span>|<span data-ttu-id="4b8f4-194">String</span><span class="sxs-lookup"><span data-stu-id="4b8f4-194">String</span></span>|<span data-ttu-id="4b8f4-195">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="4b8f4-195">The internal committed content version.</span></span> <span data-ttu-id="4b8f4-196">Наследуется от объекта [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="4b8f4-196">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="4b8f4-197">fileName</span><span class="sxs-lookup"><span data-stu-id="4b8f4-197">fileName</span></span>|<span data-ttu-id="4b8f4-198">String</span><span class="sxs-lookup"><span data-stu-id="4b8f4-198">String</span></span>|<span data-ttu-id="4b8f4-199">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="4b8f4-199">The name of the main Lob application file.</span></span> <span data-ttu-id="4b8f4-200">Наследуется от объекта [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="4b8f4-200">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="4b8f4-201">size</span><span class="sxs-lookup"><span data-stu-id="4b8f4-201">size</span></span>|<span data-ttu-id="4b8f4-202">Int64</span><span class="sxs-lookup"><span data-stu-id="4b8f4-202">Int64</span></span>|<span data-ttu-id="4b8f4-203">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="4b8f4-203">The total size, including all uploaded files.</span></span> <span data-ttu-id="4b8f4-204">Наследуется от объекта [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="4b8f4-204">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="4b8f4-205">packageId</span><span class="sxs-lookup"><span data-stu-id="4b8f4-205">packageId</span></span>|<span data-ttu-id="4b8f4-206">String</span><span class="sxs-lookup"><span data-stu-id="4b8f4-206">String</span></span>|<span data-ttu-id="4b8f4-207">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="4b8f4-207">The package identifier.</span></span>|
|<span data-ttu-id="4b8f4-208">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4b8f4-208">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="4b8f4-209">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4b8f4-209">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="4b8f4-210">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="4b8f4-210">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="4b8f4-211">versionName</span><span class="sxs-lookup"><span data-stu-id="4b8f4-211">versionName</span></span>|<span data-ttu-id="4b8f4-212">String</span><span class="sxs-lookup"><span data-stu-id="4b8f4-212">String</span></span>|<span data-ttu-id="4b8f4-213">Имя версии управляемого бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="4b8f4-213">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="4b8f4-214">versionCode</span><span class="sxs-lookup"><span data-stu-id="4b8f4-214">versionCode</span></span>|<span data-ttu-id="4b8f4-215">String</span><span class="sxs-lookup"><span data-stu-id="4b8f4-215">String</span></span>|<span data-ttu-id="4b8f4-216">Код версии управляемого бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="4b8f4-216">The version code of managed Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="4b8f4-217">Ответ</span><span class="sxs-lookup"><span data-stu-id="4b8f4-217">Response</span></span>
<span data-ttu-id="4b8f4-218">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4b8f4-218">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_apps_managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b8f4-219">Пример</span><span class="sxs-lookup"><span data-stu-id="4b8f4-219">Example</span></span>
### <a name="request"></a><span data-ttu-id="4b8f4-220">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b8f4-220">Request</span></span>
<span data-ttu-id="4b8f4-221">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b8f4-221">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4b8f4-222">Ответ</span><span class="sxs-lookup"><span data-stu-id="4b8f4-222">Response</span></span>
<span data-ttu-id="4b8f4-p120">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4b8f4-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



