# <a name="update-ioslobapp"></a><span data-ttu-id="ffb2a-101">Update iosLobApp</span><span class="sxs-lookup"><span data-stu-id="ffb2a-101">Update iosLobApp</span></span>

> <span data-ttu-id="ffb2a-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ffb2a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ffb2a-103">Обновление свойств объекта [iosLobApp](../resources/intune_apps_ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ffb2a-103">Update the properties of a [calendar](../resources/intune_apps_ioslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ffb2a-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="ffb2a-104">Prerequisites</span></span>
<span data-ttu-id="ffb2a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ffb2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ffb2a-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ffb2a-107">Permission type</span></span>|<span data-ttu-id="ffb2a-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ffb2a-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ffb2a-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ffb2a-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ffb2a-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffb2a-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ffb2a-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ffb2a-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ffb2a-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffb2a-112">Not supported.</span></span>|
|<span data-ttu-id="ffb2a-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ffb2a-113">Application</span></span>|<span data-ttu-id="ffb2a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffb2a-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ffb2a-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ffb2a-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="ffb2a-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ffb2a-116">Request headers</span></span>
|<span data-ttu-id="ffb2a-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ffb2a-117">Header</span></span>|<span data-ttu-id="ffb2a-118">Значение</span><span class="sxs-lookup"><span data-stu-id="ffb2a-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ffb2a-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="ffb2a-119">Authorization</span></span>|<span data-ttu-id="ffb2a-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ffb2a-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ffb2a-121">Accept</span><span class="sxs-lookup"><span data-stu-id="ffb2a-121">Accept</span></span>|<span data-ttu-id="ffb2a-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ffb2a-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ffb2a-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ffb2a-123">Request body</span></span>
<span data-ttu-id="ffb2a-124">В теле запроса добавьте представление объекта [iosLobApp](../resources/intune_apps_ioslobapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ffb2a-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_apps_ioslobapp.md) object.</span></span>

<span data-ttu-id="ffb2a-125">Ниже показаны свойства, которые необходимо указывать при создании объекта [iosLobApp](../resources/intune_apps_ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ffb2a-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="ffb2a-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="ffb2a-126">Property</span></span>|<span data-ttu-id="ffb2a-127">Тип</span><span class="sxs-lookup"><span data-stu-id="ffb2a-127">Type</span></span>|<span data-ttu-id="ffb2a-128">Описание</span><span class="sxs-lookup"><span data-stu-id="ffb2a-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffb2a-129">id</span><span class="sxs-lookup"><span data-stu-id="ffb2a-129">id</span></span>|<span data-ttu-id="ffb2a-130">String</span><span class="sxs-lookup"><span data-stu-id="ffb2a-130">String</span></span>|<span data-ttu-id="ffb2a-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ffb2a-131">Key of the setting.</span></span> <span data-ttu-id="ffb2a-132">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ffb2a-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ffb2a-133">displayName</span><span class="sxs-lookup"><span data-stu-id="ffb2a-133">displayName</span></span>|<span data-ttu-id="ffb2a-134">String</span><span class="sxs-lookup"><span data-stu-id="ffb2a-134">String</span></span>|<span data-ttu-id="ffb2a-135">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="ffb2a-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ffb2a-136">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ffb2a-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ffb2a-137">description</span><span class="sxs-lookup"><span data-stu-id="ffb2a-137">description</span></span>|<span data-ttu-id="ffb2a-138">String</span><span class="sxs-lookup"><span data-stu-id="ffb2a-138">String</span></span>|<span data-ttu-id="ffb2a-139">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="ffb2a-139">The description of the app.</span></span> <span data-ttu-id="ffb2a-140">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ffb2a-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ffb2a-141">publisher</span><span class="sxs-lookup"><span data-stu-id="ffb2a-141">Publisher</span></span>|<span data-ttu-id="ffb2a-142">String</span><span class="sxs-lookup"><span data-stu-id="ffb2a-142">String</span></span>|<span data-ttu-id="ffb2a-143">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="ffb2a-143">The name of the app.</span></span> <span data-ttu-id="ffb2a-144">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ffb2a-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ffb2a-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ffb2a-145">largeIcon</span></span>|[<span data-ttu-id="ffb2a-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ffb2a-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="ffb2a-147">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="ffb2a-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ffb2a-148">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ffb2a-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ffb2a-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ffb2a-149">createdDateTime</span></span>|<span data-ttu-id="ffb2a-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ffb2a-150">DateTimeOffset</span></span>|<span data-ttu-id="ffb2a-151">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="ffb2a-151">The date and time the group was created.</span></span> <span data-ttu-id="ffb2a-152">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ffb2a-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ffb2a-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ffb2a-153">lastModifiedDateTime</span></span>|<span data-ttu-id="ffb2a-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ffb2a-154">DateTimeOffset</span></span>|<span data-ttu-id="ffb2a-155">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="ffb2a-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="ffb2a-156">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ffb2a-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ffb2a-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ffb2a-157">isFeatured</span></span>|<span data-ttu-id="ffb2a-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffb2a-158">Boolean</span></span>|<span data-ttu-id="ffb2a-159">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ffb2a-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ffb2a-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ffb2a-160">privacyInformationUrl</span></span>|<span data-ttu-id="ffb2a-161">String</span><span class="sxs-lookup"><span data-stu-id="ffb2a-161">String</span></span>|<span data-ttu-id="ffb2a-162">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="ffb2a-162">The privacy statement Url.</span></span> <span data-ttu-id="ffb2a-163">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ffb2a-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ffb2a-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ffb2a-164">informationUrl</span></span>|<span data-ttu-id="ffb2a-165">String</span><span class="sxs-lookup"><span data-stu-id="ffb2a-165">String</span></span>|<span data-ttu-id="ffb2a-166">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="ffb2a-166">The more information Url.</span></span> <span data-ttu-id="ffb2a-167">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ffb2a-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ffb2a-168">owner</span><span class="sxs-lookup"><span data-stu-id="ffb2a-168">owner</span></span>|<span data-ttu-id="ffb2a-169">String</span><span class="sxs-lookup"><span data-stu-id="ffb2a-169">String</span></span>|<span data-ttu-id="ffb2a-170">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="ffb2a-170">The owner of the app.</span></span> <span data-ttu-id="ffb2a-171">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ffb2a-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ffb2a-172">developer</span><span class="sxs-lookup"><span data-stu-id="ffb2a-172">developer</span></span>|<span data-ttu-id="ffb2a-173">String</span><span class="sxs-lookup"><span data-stu-id="ffb2a-173">String</span></span>|<span data-ttu-id="ffb2a-174">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="ffb2a-174">The name of the app.</span></span> <span data-ttu-id="ffb2a-175">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ffb2a-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ffb2a-176">notes</span><span class="sxs-lookup"><span data-stu-id="ffb2a-176">Notes</span></span>|<span data-ttu-id="ffb2a-177">String</span><span class="sxs-lookup"><span data-stu-id="ffb2a-177">String</span></span>|<span data-ttu-id="ffb2a-178">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="ffb2a-178">Notes for the app.</span></span> <span data-ttu-id="ffb2a-179">Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ffb2a-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ffb2a-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="ffb2a-180">publishingState</span></span>|<span data-ttu-id="ffb2a-181">String</span><span class="sxs-lookup"><span data-stu-id="ffb2a-181">String</span></span>|<span data-ttu-id="ffb2a-182">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="ffb2a-182">The publishing state for the app.</span></span> <span data-ttu-id="ffb2a-183">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="ffb2a-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ffb2a-184">Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md). Допустимые значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="ffb2a-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ffb2a-185">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="ffb2a-185">committedContentVersion</span></span>|<span data-ttu-id="ffb2a-186">String</span><span class="sxs-lookup"><span data-stu-id="ffb2a-186">String</span></span>|<span data-ttu-id="ffb2a-187">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="ffb2a-187">The internal committed content version.</span></span> <span data-ttu-id="ffb2a-188">Наследуется от [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ffb2a-188">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="ffb2a-189">fileName</span><span class="sxs-lookup"><span data-stu-id="ffb2a-189">fileName</span></span>|<span data-ttu-id="ffb2a-190">String</span><span class="sxs-lookup"><span data-stu-id="ffb2a-190">String</span></span>|<span data-ttu-id="ffb2a-191">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="ffb2a-191">The name of the main Lob application file.</span></span> <span data-ttu-id="ffb2a-192">Наследуется от [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ffb2a-192">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="ffb2a-193">size</span><span class="sxs-lookup"><span data-stu-id="ffb2a-193">size</span></span>|<span data-ttu-id="ffb2a-194">Int64</span><span class="sxs-lookup"><span data-stu-id="ffb2a-194">Int64</span></span>|<span data-ttu-id="ffb2a-195">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="ffb2a-195">The total size, including all uploaded files.</span></span> <span data-ttu-id="ffb2a-196">Наследуется от [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ffb2a-196">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="ffb2a-197">bundleId</span><span class="sxs-lookup"><span data-stu-id="ffb2a-197">bundleId</span></span>|<span data-ttu-id="ffb2a-198">String</span><span class="sxs-lookup"><span data-stu-id="ffb2a-198">String</span></span>|<span data-ttu-id="ffb2a-199">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="ffb2a-199">The Identity Name.</span></span>|
|<span data-ttu-id="ffb2a-200">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="ffb2a-200">applicableDeviceType</span></span>|[<span data-ttu-id="ffb2a-201">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="ffb2a-201">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="ffb2a-202">Архитектура iOS, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="ffb2a-202">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="ffb2a-203">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ffb2a-203">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="ffb2a-204">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ffb2a-204">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="ffb2a-205">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="ffb2a-205">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="ffb2a-206">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ffb2a-206">expirationDateTime</span></span>|<span data-ttu-id="ffb2a-207">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ffb2a-207">DateTimeOffset</span></span>|<span data-ttu-id="ffb2a-208">Срок действия.</span><span class="sxs-lookup"><span data-stu-id="ffb2a-208">: The expiration time for the subscription.</span></span>|
|<span data-ttu-id="ffb2a-209">versionNumber</span><span class="sxs-lookup"><span data-stu-id="ffb2a-209">versionNumber</span></span>|<span data-ttu-id="ffb2a-210">String</span><span class="sxs-lookup"><span data-stu-id="ffb2a-210">String</span></span>|<span data-ttu-id="ffb2a-211">Номер версии бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="ffb2a-211">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="ffb2a-212">buildNumber</span><span class="sxs-lookup"><span data-stu-id="ffb2a-212">buildNumber</span></span>|<span data-ttu-id="ffb2a-213">String</span><span class="sxs-lookup"><span data-stu-id="ffb2a-213">String</span></span>|<span data-ttu-id="ffb2a-214">Номер сборки бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="ffb2a-214">The build number of iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="ffb2a-215">Ответ</span><span class="sxs-lookup"><span data-stu-id="ffb2a-215">Response</span></span>
<span data-ttu-id="ffb2a-216">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [iosLobApp](../resources/intune_apps_ioslobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ffb2a-216">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_apps_ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ffb2a-217">Пример</span><span class="sxs-lookup"><span data-stu-id="ffb2a-217">Example</span></span>
### <a name="request"></a><span data-ttu-id="ffb2a-218">Запрос</span><span class="sxs-lookup"><span data-stu-id="ffb2a-218">Request</span></span>
<span data-ttu-id="ffb2a-219">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ffb2a-219">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1205

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

### <a name="response"></a><span data-ttu-id="ffb2a-220">Ответ</span><span class="sxs-lookup"><span data-stu-id="ffb2a-220">Response</span></span>
<span data-ttu-id="ffb2a-p118">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ffb2a-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1361

{
  "@odata.type": "#microsoft.graph.iosLobApp",
  "id": "b34052ea-52ea-b340-ea52-40b3ea5240b3",
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



