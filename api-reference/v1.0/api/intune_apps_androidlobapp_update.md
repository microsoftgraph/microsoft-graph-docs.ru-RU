# <a name="update-androidlobapp"></a><span data-ttu-id="fb5d5-101">Update androidLobApp</span><span class="sxs-lookup"><span data-stu-id="fb5d5-101">Update androidLobApp</span></span>

> <span data-ttu-id="fb5d5-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fb5d5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fb5d5-103">Обновление свойств объекта [androidLobApp](../resources/intune_apps_androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="fb5d5-103">Update the properties of a [calendar](../resources/intune_apps_androidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fb5d5-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="fb5d5-104">Prerequisites</span></span>
<span data-ttu-id="fb5d5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fb5d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fb5d5-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fb5d5-107">Permission type</span></span>|<span data-ttu-id="fb5d5-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fb5d5-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb5d5-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fb5d5-109">Delegated (work or school account)</span></span>|<span data-ttu-id="fb5d5-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb5d5-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fb5d5-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fb5d5-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb5d5-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb5d5-112">Not supported.</span></span>|
|<span data-ttu-id="fb5d5-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fb5d5-113">Application</span></span>|<span data-ttu-id="fb5d5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb5d5-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb5d5-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fb5d5-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="fb5d5-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fb5d5-116">Request headers</span></span>
|<span data-ttu-id="fb5d5-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fb5d5-117">Header</span></span>|<span data-ttu-id="fb5d5-118">Значение</span><span class="sxs-lookup"><span data-stu-id="fb5d5-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb5d5-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb5d5-119">Authorization</span></span>|<span data-ttu-id="fb5d5-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fb5d5-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="fb5d5-121">Accept</span><span class="sxs-lookup"><span data-stu-id="fb5d5-121">Accept</span></span>|<span data-ttu-id="fb5d5-122">application/json</span><span class="sxs-lookup"><span data-stu-id="fb5d5-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb5d5-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fb5d5-123">Request body</span></span>
<span data-ttu-id="fb5d5-124">В теле запроса добавьте представление объекта [androidLobApp](../resources/intune_apps_androidlobapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fb5d5-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_apps_androidlobapp.md) object.</span></span>

<span data-ttu-id="fb5d5-125">Ниже показаны свойства, которые необходимо указывать при создании объекта [androidLobApp](../resources/intune_apps_androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="fb5d5-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="fb5d5-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="fb5d5-126">Property</span></span>|<span data-ttu-id="fb5d5-127">Тип</span><span class="sxs-lookup"><span data-stu-id="fb5d5-127">Type</span></span>|<span data-ttu-id="fb5d5-128">Описание</span><span class="sxs-lookup"><span data-stu-id="fb5d5-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb5d5-129">id</span><span class="sxs-lookup"><span data-stu-id="fb5d5-129">id</span></span>|<span data-ttu-id="fb5d5-130">String</span><span class="sxs-lookup"><span data-stu-id="fb5d5-130">String</span></span>|<span data-ttu-id="fb5d5-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fb5d5-131">Key of the setting.</span></span> <span data-ttu-id="fb5d5-132">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fb5d5-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fb5d5-133">displayName</span><span class="sxs-lookup"><span data-stu-id="fb5d5-133">displayName</span></span>|<span data-ttu-id="fb5d5-134">String</span><span class="sxs-lookup"><span data-stu-id="fb5d5-134">String</span></span>|<span data-ttu-id="fb5d5-135">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="fb5d5-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="fb5d5-136">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fb5d5-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fb5d5-137">description</span><span class="sxs-lookup"><span data-stu-id="fb5d5-137">description</span></span>|<span data-ttu-id="fb5d5-138">String</span><span class="sxs-lookup"><span data-stu-id="fb5d5-138">String</span></span>|<span data-ttu-id="fb5d5-139">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="fb5d5-139">The description of the app.</span></span> <span data-ttu-id="fb5d5-140">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fb5d5-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fb5d5-141">publisher</span><span class="sxs-lookup"><span data-stu-id="fb5d5-141">Publisher</span></span>|<span data-ttu-id="fb5d5-142">String</span><span class="sxs-lookup"><span data-stu-id="fb5d5-142">String</span></span>|<span data-ttu-id="fb5d5-143">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="fb5d5-143">The name of the app.</span></span> <span data-ttu-id="fb5d5-144">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fb5d5-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fb5d5-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="fb5d5-145">largeIcon</span></span>|[<span data-ttu-id="fb5d5-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="fb5d5-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="fb5d5-147">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="fb5d5-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="fb5d5-148">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fb5d5-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fb5d5-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fb5d5-149">createdDateTime</span></span>|<span data-ttu-id="fb5d5-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb5d5-150">DateTimeOffset</span></span>|<span data-ttu-id="fb5d5-151">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="fb5d5-151">The date and time the group was created.</span></span> <span data-ttu-id="fb5d5-152">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fb5d5-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fb5d5-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fb5d5-153">lastModifiedDateTime</span></span>|<span data-ttu-id="fb5d5-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb5d5-154">DateTimeOffset</span></span>|<span data-ttu-id="fb5d5-155">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="fb5d5-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="fb5d5-156">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fb5d5-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fb5d5-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="fb5d5-157">isFeatured</span></span>|<span data-ttu-id="fb5d5-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb5d5-158">Boolean</span></span>|<span data-ttu-id="fb5d5-159">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fb5d5-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fb5d5-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="fb5d5-160">privacyInformationUrl</span></span>|<span data-ttu-id="fb5d5-161">String</span><span class="sxs-lookup"><span data-stu-id="fb5d5-161">String</span></span>|<span data-ttu-id="fb5d5-162">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="fb5d5-162">The privacy statement Url.</span></span> <span data-ttu-id="fb5d5-163">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fb5d5-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fb5d5-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="fb5d5-164">informationUrl</span></span>|<span data-ttu-id="fb5d5-165">String</span><span class="sxs-lookup"><span data-stu-id="fb5d5-165">String</span></span>|<span data-ttu-id="fb5d5-166">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="fb5d5-166">The more information Url.</span></span> <span data-ttu-id="fb5d5-167">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fb5d5-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fb5d5-168">owner</span><span class="sxs-lookup"><span data-stu-id="fb5d5-168">owner</span></span>|<span data-ttu-id="fb5d5-169">String</span><span class="sxs-lookup"><span data-stu-id="fb5d5-169">String</span></span>|<span data-ttu-id="fb5d5-170">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="fb5d5-170">The owner of the app.</span></span> <span data-ttu-id="fb5d5-171">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fb5d5-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fb5d5-172">developer</span><span class="sxs-lookup"><span data-stu-id="fb5d5-172">developer</span></span>|<span data-ttu-id="fb5d5-173">String</span><span class="sxs-lookup"><span data-stu-id="fb5d5-173">String</span></span>|<span data-ttu-id="fb5d5-174">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="fb5d5-174">The name of the app.</span></span> <span data-ttu-id="fb5d5-175">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fb5d5-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fb5d5-176">notes</span><span class="sxs-lookup"><span data-stu-id="fb5d5-176">Notes</span></span>|<span data-ttu-id="fb5d5-177">String</span><span class="sxs-lookup"><span data-stu-id="fb5d5-177">String</span></span>|<span data-ttu-id="fb5d5-178">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="fb5d5-178">Notes for the app.</span></span> <span data-ttu-id="fb5d5-179">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fb5d5-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fb5d5-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="fb5d5-180">publishingState</span></span>|<span data-ttu-id="fb5d5-181">String</span><span class="sxs-lookup"><span data-stu-id="fb5d5-181">String</span></span>|<span data-ttu-id="fb5d5-182">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="fb5d5-182">The publishing state for the app.</span></span> <span data-ttu-id="fb5d5-183">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="fb5d5-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="fb5d5-184">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md). Допустимые значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="fb5d5-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="fb5d5-185">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="fb5d5-185">committedContentVersion</span></span>|<span data-ttu-id="fb5d5-186">String</span><span class="sxs-lookup"><span data-stu-id="fb5d5-186">String</span></span>|<span data-ttu-id="fb5d5-187">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="fb5d5-187">The internal committed content version.</span></span> <span data-ttu-id="fb5d5-188">Наследуется от [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="fb5d5-188">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="fb5d5-189">fileName</span><span class="sxs-lookup"><span data-stu-id="fb5d5-189">fileName</span></span>|<span data-ttu-id="fb5d5-190">String</span><span class="sxs-lookup"><span data-stu-id="fb5d5-190">String</span></span>|<span data-ttu-id="fb5d5-191">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="fb5d5-191">The name of the main Lob application file.</span></span> <span data-ttu-id="fb5d5-192">Наследуется от [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="fb5d5-192">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="fb5d5-193">size</span><span class="sxs-lookup"><span data-stu-id="fb5d5-193">size</span></span>|<span data-ttu-id="fb5d5-194">Int64</span><span class="sxs-lookup"><span data-stu-id="fb5d5-194">Int64</span></span>|<span data-ttu-id="fb5d5-195">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="fb5d5-195">The total size, including all uploaded files.</span></span> <span data-ttu-id="fb5d5-196">Наследуется от [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="fb5d5-196">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="fb5d5-197">packageId</span><span class="sxs-lookup"><span data-stu-id="fb5d5-197">packageId</span></span>|<span data-ttu-id="fb5d5-198">String</span><span class="sxs-lookup"><span data-stu-id="fb5d5-198">String</span></span>|<span data-ttu-id="fb5d5-199">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="fb5d5-199">The package identifier.</span></span>|
|<span data-ttu-id="fb5d5-200">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="fb5d5-200">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="fb5d5-201">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="fb5d5-201">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="fb5d5-202">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="fb5d5-202">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="fb5d5-203">versionName</span><span class="sxs-lookup"><span data-stu-id="fb5d5-203">versionName</span></span>|<span data-ttu-id="fb5d5-204">String</span><span class="sxs-lookup"><span data-stu-id="fb5d5-204">String</span></span>|<span data-ttu-id="fb5d5-205">Имя версии бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="fb5d5-205">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="fb5d5-206">versionCode</span><span class="sxs-lookup"><span data-stu-id="fb5d5-206">versionCode</span></span>|<span data-ttu-id="fb5d5-207">String</span><span class="sxs-lookup"><span data-stu-id="fb5d5-207">String</span></span>|<span data-ttu-id="fb5d5-208">Код версии бизнес-приложения Android.</span><span class="sxs-lookup"><span data-stu-id="fb5d5-208">The version code of Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="fb5d5-209">Ответ</span><span class="sxs-lookup"><span data-stu-id="fb5d5-209">Response</span></span>
<span data-ttu-id="fb5d5-210">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [androidLobApp](../resources/intune_apps_androidlobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="fb5d5-210">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_apps_androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb5d5-211">Пример</span><span class="sxs-lookup"><span data-stu-id="fb5d5-211">Example</span></span>
### <a name="request"></a><span data-ttu-id="fb5d5-212">Запрос</span><span class="sxs-lookup"><span data-stu-id="fb5d5-212">Request</span></span>
<span data-ttu-id="fb5d5-213">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fb5d5-213">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1087

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

### <a name="response"></a><span data-ttu-id="fb5d5-214">Ответ</span><span class="sxs-lookup"><span data-stu-id="fb5d5-214">Response</span></span>
<span data-ttu-id="fb5d5-p118">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fb5d5-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1247

{
  "@odata.type": "#microsoft.graph.androidLobApp",
  "id": "4b9a27d0-27d0-4b9a-d027-9a4bd0279a4b",
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



