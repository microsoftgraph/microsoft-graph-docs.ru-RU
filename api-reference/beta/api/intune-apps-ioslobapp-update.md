---
title: Update iosLobApp
description: Обновление свойств объекта iosLobApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 339f09af9617f97f73d5560b26447b045c4ba532
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158403"
---
# <a name="update-ioslobapp"></a><span data-ttu-id="9178f-103">Update iosLobApp</span><span class="sxs-lookup"><span data-stu-id="9178f-103">Update iosLobApp</span></span>

> <span data-ttu-id="9178f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9178f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9178f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9178f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9178f-106">Обновление свойств объекта [iosLobApp](../resources/intune-apps-ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="9178f-106">Update the properties of a [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9178f-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="9178f-107">Prerequisites</span></span>
<span data-ttu-id="9178f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9178f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9178f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9178f-110">Permission type</span></span>|<span data-ttu-id="9178f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9178f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9178f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9178f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9178f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9178f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9178f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9178f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9178f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9178f-115">Not supported.</span></span>|
|<span data-ttu-id="9178f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9178f-116">Application</span></span>|<span data-ttu-id="9178f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9178f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9178f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9178f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="9178f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9178f-119">Request headers</span></span>
|<span data-ttu-id="9178f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9178f-120">Header</span></span>|<span data-ttu-id="9178f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9178f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9178f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9178f-122">Authorization</span></span>|<span data-ttu-id="9178f-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="9178f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9178f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9178f-124">Accept</span></span>|<span data-ttu-id="9178f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9178f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9178f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9178f-126">Request body</span></span>
<span data-ttu-id="9178f-127">В теле запроса добавьте представление объекта [iosLobApp](../resources/intune-apps-ioslobapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9178f-127">In the request body, supply a JSON representation for the [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

<span data-ttu-id="9178f-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [iosLobApp](../resources/intune-apps-ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="9178f-128">The following table shows the properties that are required when you create the [iosLobApp](../resources/intune-apps-ioslobapp.md).</span></span>

|<span data-ttu-id="9178f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="9178f-129">Property</span></span>|<span data-ttu-id="9178f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9178f-130">Type</span></span>|<span data-ttu-id="9178f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9178f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9178f-132">id</span><span class="sxs-lookup"><span data-stu-id="9178f-132">id</span></span>|<span data-ttu-id="9178f-133">Строка</span><span class="sxs-lookup"><span data-stu-id="9178f-133">String</span></span>|<span data-ttu-id="9178f-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9178f-134">Key of the entity.</span></span> <span data-ttu-id="9178f-135">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9178f-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9178f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="9178f-136">displayName</span></span>|<span data-ttu-id="9178f-137">String</span><span class="sxs-lookup"><span data-stu-id="9178f-137">String</span></span>|<span data-ttu-id="9178f-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="9178f-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="9178f-139">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9178f-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9178f-140">description</span><span class="sxs-lookup"><span data-stu-id="9178f-140">description</span></span>|<span data-ttu-id="9178f-141">Строка</span><span class="sxs-lookup"><span data-stu-id="9178f-141">String</span></span>|<span data-ttu-id="9178f-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="9178f-142">The description of the app.</span></span> <span data-ttu-id="9178f-143">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9178f-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9178f-144">publisher</span><span class="sxs-lookup"><span data-stu-id="9178f-144">publisher</span></span>|<span data-ttu-id="9178f-145">String</span><span class="sxs-lookup"><span data-stu-id="9178f-145">String</span></span>|<span data-ttu-id="9178f-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="9178f-146">The publisher of the app.</span></span> <span data-ttu-id="9178f-147">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9178f-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9178f-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="9178f-148">largeIcon</span></span>|[<span data-ttu-id="9178f-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9178f-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9178f-150">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="9178f-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="9178f-151">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9178f-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9178f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9178f-152">createdDateTime</span></span>|<span data-ttu-id="9178f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9178f-153">DateTimeOffset</span></span>|<span data-ttu-id="9178f-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="9178f-154">The date and time the app was created.</span></span> <span data-ttu-id="9178f-155">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9178f-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9178f-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9178f-156">lastModifiedDateTime</span></span>|<span data-ttu-id="9178f-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9178f-157">DateTimeOffset</span></span>|<span data-ttu-id="9178f-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="9178f-158">The date and time the app was last modified.</span></span> <span data-ttu-id="9178f-159">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9178f-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9178f-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="9178f-160">isFeatured</span></span>|<span data-ttu-id="9178f-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="9178f-161">Boolean</span></span>|<span data-ttu-id="9178f-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9178f-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9178f-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="9178f-163">privacyInformationUrl</span></span>|<span data-ttu-id="9178f-164">String</span><span class="sxs-lookup"><span data-stu-id="9178f-164">String</span></span>|<span data-ttu-id="9178f-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="9178f-165">The privacy statement Url.</span></span> <span data-ttu-id="9178f-166">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9178f-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9178f-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="9178f-167">informationUrl</span></span>|<span data-ttu-id="9178f-168">String</span><span class="sxs-lookup"><span data-stu-id="9178f-168">String</span></span>|<span data-ttu-id="9178f-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="9178f-169">The more information Url.</span></span> <span data-ttu-id="9178f-170">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9178f-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9178f-171">owner</span><span class="sxs-lookup"><span data-stu-id="9178f-171">owner</span></span>|<span data-ttu-id="9178f-172">Строка</span><span class="sxs-lookup"><span data-stu-id="9178f-172">String</span></span>|<span data-ttu-id="9178f-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="9178f-173">The owner of the app.</span></span> <span data-ttu-id="9178f-174">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9178f-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9178f-175">developer</span><span class="sxs-lookup"><span data-stu-id="9178f-175">developer</span></span>|<span data-ttu-id="9178f-176">String</span><span class="sxs-lookup"><span data-stu-id="9178f-176">String</span></span>|<span data-ttu-id="9178f-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="9178f-177">The developer of the app.</span></span> <span data-ttu-id="9178f-178">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9178f-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9178f-179">notes</span><span class="sxs-lookup"><span data-stu-id="9178f-179">notes</span></span>|<span data-ttu-id="9178f-180">String</span><span class="sxs-lookup"><span data-stu-id="9178f-180">String</span></span>|<span data-ttu-id="9178f-181">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="9178f-181">Notes for the app.</span></span> <span data-ttu-id="9178f-182">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9178f-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9178f-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="9178f-183">uploadState</span></span>|<span data-ttu-id="9178f-184">Int32</span><span class="sxs-lookup"><span data-stu-id="9178f-184">Int32</span></span>|<span data-ttu-id="9178f-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="9178f-185">The upload state.</span></span> <span data-ttu-id="9178f-186">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9178f-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9178f-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="9178f-187">publishingState</span></span>|[<span data-ttu-id="9178f-188">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="9178f-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="9178f-189">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="9178f-189">The publishing state for the app.</span></span> <span data-ttu-id="9178f-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="9178f-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="9178f-191">НаСледуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9178f-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="9178f-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="9178f-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="9178f-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="9178f-193">isAssigned</span></span>|<span data-ttu-id="9178f-194">Логический</span><span class="sxs-lookup"><span data-stu-id="9178f-194">Boolean</span></span>|<span data-ttu-id="9178f-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="9178f-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="9178f-196">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9178f-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9178f-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9178f-197">roleScopeTagIds</span></span>|<span data-ttu-id="9178f-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9178f-198">String collection</span></span>|<span data-ttu-id="9178f-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="9178f-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="9178f-200">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9178f-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9178f-201">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="9178f-201">committedContentVersion</span></span>|<span data-ttu-id="9178f-202">String</span><span class="sxs-lookup"><span data-stu-id="9178f-202">String</span></span>|<span data-ttu-id="9178f-203">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="9178f-203">The internal committed content version.</span></span> <span data-ttu-id="9178f-204">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="9178f-204">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9178f-205">fileName</span><span class="sxs-lookup"><span data-stu-id="9178f-205">fileName</span></span>|<span data-ttu-id="9178f-206">String</span><span class="sxs-lookup"><span data-stu-id="9178f-206">String</span></span>|<span data-ttu-id="9178f-207">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="9178f-207">The name of the main Lob application file.</span></span> <span data-ttu-id="9178f-208">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="9178f-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9178f-209">size</span><span class="sxs-lookup"><span data-stu-id="9178f-209">size</span></span>|<span data-ttu-id="9178f-210">Int64</span><span class="sxs-lookup"><span data-stu-id="9178f-210">Int64</span></span>|<span data-ttu-id="9178f-211">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="9178f-211">The total size, including all uploaded files.</span></span> <span data-ttu-id="9178f-212">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="9178f-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9178f-213">bundleId</span><span class="sxs-lookup"><span data-stu-id="9178f-213">bundleId</span></span>|<span data-ttu-id="9178f-214">String</span><span class="sxs-lookup"><span data-stu-id="9178f-214">String</span></span>|<span data-ttu-id="9178f-215">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="9178f-215">The Identity Name.</span></span>|
|<span data-ttu-id="9178f-216">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="9178f-216">applicableDeviceType</span></span>|[<span data-ttu-id="9178f-217">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="9178f-217">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="9178f-218">Архитектура iOS, поддерживаемая этим приложением.</span><span class="sxs-lookup"><span data-stu-id="9178f-218">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="9178f-219">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9178f-219">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="9178f-220">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9178f-220">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="9178f-221">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="9178f-221">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="9178f-222">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="9178f-222">expirationDateTime</span></span>|<span data-ttu-id="9178f-223">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9178f-223">DateTimeOffset</span></span>|<span data-ttu-id="9178f-224">Время окончания срока действия.</span><span class="sxs-lookup"><span data-stu-id="9178f-224">The expiration time.</span></span>|
|<span data-ttu-id="9178f-225">versionNumber</span><span class="sxs-lookup"><span data-stu-id="9178f-225">versionNumber</span></span>|<span data-ttu-id="9178f-226">String</span><span class="sxs-lookup"><span data-stu-id="9178f-226">String</span></span>|<span data-ttu-id="9178f-227">Номер версии бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="9178f-227">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="9178f-228">buildNumber</span><span class="sxs-lookup"><span data-stu-id="9178f-228">buildNumber</span></span>|<span data-ttu-id="9178f-229">String</span><span class="sxs-lookup"><span data-stu-id="9178f-229">String</span></span>|<span data-ttu-id="9178f-230">Номер сборки бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="9178f-230">The build number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="9178f-231">identityVersion</span><span class="sxs-lookup"><span data-stu-id="9178f-231">identityVersion</span></span>|<span data-ttu-id="9178f-232">String</span><span class="sxs-lookup"><span data-stu-id="9178f-232">String</span></span>|<span data-ttu-id="9178f-233">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="9178f-233">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="9178f-234">Ответ</span><span class="sxs-lookup"><span data-stu-id="9178f-234">Response</span></span>
<span data-ttu-id="9178f-235">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [iosLobApp](../resources/intune-apps-ioslobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9178f-235">If successful, this method returns a `200 OK` response code and an updated [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9178f-236">Пример</span><span class="sxs-lookup"><span data-stu-id="9178f-236">Example</span></span>

### <a name="request"></a><span data-ttu-id="9178f-237">Запрос</span><span class="sxs-lookup"><span data-stu-id="9178f-237">Request</span></span>
<span data-ttu-id="9178f-238">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9178f-238">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1364

{
  "@odata.type": "#microsoft.graph.iosLobApp",
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
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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
    "v11_0": true,
    "v12_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="9178f-239">Отклик</span><span class="sxs-lookup"><span data-stu-id="9178f-239">Response</span></span>
<span data-ttu-id="9178f-p121">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9178f-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1536

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
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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
    "v11_0": true,
    "v12_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```




