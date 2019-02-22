---
title: Обновление Виндовсфонексап
description: Обновление свойств объекта Виндовсфонексап.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 096e7430d0f1e544b5fbd4a9475b70e45ecb0719
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150038"
---
# <a name="update-windowsphonexap"></a><span data-ttu-id="5a887-103">Обновление Виндовсфонексап</span><span class="sxs-lookup"><span data-stu-id="5a887-103">Update windowsPhoneXAP</span></span>

> <span data-ttu-id="5a887-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a887-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5a887-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5a887-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a887-106">Обновление свойств объекта [виндовсфонексап](../resources/intune-apps-windowsphonexap.md) .</span><span class="sxs-lookup"><span data-stu-id="5a887-106">Update the properties of a [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5a887-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5a887-107">Prerequisites</span></span>
<span data-ttu-id="5a887-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5a887-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5a887-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5a887-110">Permission type</span></span>|<span data-ttu-id="5a887-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5a887-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a887-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5a887-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5a887-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a887-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5a887-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5a887-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a887-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a887-115">Not supported.</span></span>|
|<span data-ttu-id="5a887-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5a887-116">Application</span></span>|<span data-ttu-id="5a887-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a887-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a887-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5a887-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="5a887-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5a887-119">Request headers</span></span>
|<span data-ttu-id="5a887-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5a887-120">Header</span></span>|<span data-ttu-id="5a887-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5a887-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a887-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5a887-122">Authorization</span></span>|<span data-ttu-id="5a887-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5a887-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a887-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5a887-124">Accept</span></span>|<span data-ttu-id="5a887-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5a887-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a887-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5a887-126">Request body</span></span>
<span data-ttu-id="5a887-127">В тексте запроса добавьте представление объекта [Виндовсфонексап](../resources/intune-apps-windowsphonexap.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a887-127">In the request body, supply a JSON representation for the [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object.</span></span>

<span data-ttu-id="5a887-128">В следующей таблице приведены свойства, необходимые при создании [виндовсфонексап](../resources/intune-apps-windowsphonexap.md).</span><span class="sxs-lookup"><span data-stu-id="5a887-128">The following table shows the properties that are required when you create the [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md).</span></span>

|<span data-ttu-id="5a887-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a887-129">Property</span></span>|<span data-ttu-id="5a887-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5a887-130">Type</span></span>|<span data-ttu-id="5a887-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5a887-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a887-132">id</span><span class="sxs-lookup"><span data-stu-id="5a887-132">id</span></span>|<span data-ttu-id="5a887-133">Строка</span><span class="sxs-lookup"><span data-stu-id="5a887-133">String</span></span>|<span data-ttu-id="5a887-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5a887-134">Key of the entity.</span></span> <span data-ttu-id="5a887-135">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5a887-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5a887-136">displayName</span><span class="sxs-lookup"><span data-stu-id="5a887-136">displayName</span></span>|<span data-ttu-id="5a887-137">String</span><span class="sxs-lookup"><span data-stu-id="5a887-137">String</span></span>|<span data-ttu-id="5a887-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="5a887-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="5a887-139">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5a887-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5a887-140">description</span><span class="sxs-lookup"><span data-stu-id="5a887-140">description</span></span>|<span data-ttu-id="5a887-141">Строка</span><span class="sxs-lookup"><span data-stu-id="5a887-141">String</span></span>|<span data-ttu-id="5a887-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="5a887-142">The description of the app.</span></span> <span data-ttu-id="5a887-143">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5a887-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5a887-144">publisher</span><span class="sxs-lookup"><span data-stu-id="5a887-144">publisher</span></span>|<span data-ttu-id="5a887-145">String</span><span class="sxs-lookup"><span data-stu-id="5a887-145">String</span></span>|<span data-ttu-id="5a887-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="5a887-146">The publisher of the app.</span></span> <span data-ttu-id="5a887-147">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5a887-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5a887-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="5a887-148">largeIcon</span></span>|[<span data-ttu-id="5a887-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="5a887-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="5a887-150">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="5a887-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="5a887-151">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5a887-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5a887-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5a887-152">createdDateTime</span></span>|<span data-ttu-id="5a887-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a887-153">DateTimeOffset</span></span>|<span data-ttu-id="5a887-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="5a887-154">The date and time the app was created.</span></span> <span data-ttu-id="5a887-155">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5a887-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5a887-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5a887-156">lastModifiedDateTime</span></span>|<span data-ttu-id="5a887-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a887-157">DateTimeOffset</span></span>|<span data-ttu-id="5a887-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="5a887-158">The date and time the app was last modified.</span></span> <span data-ttu-id="5a887-159">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5a887-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5a887-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="5a887-160">isFeatured</span></span>|<span data-ttu-id="5a887-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="5a887-161">Boolean</span></span>|<span data-ttu-id="5a887-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5a887-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5a887-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="5a887-163">privacyInformationUrl</span></span>|<span data-ttu-id="5a887-164">String</span><span class="sxs-lookup"><span data-stu-id="5a887-164">String</span></span>|<span data-ttu-id="5a887-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="5a887-165">The privacy statement Url.</span></span> <span data-ttu-id="5a887-166">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5a887-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5a887-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="5a887-167">informationUrl</span></span>|<span data-ttu-id="5a887-168">String</span><span class="sxs-lookup"><span data-stu-id="5a887-168">String</span></span>|<span data-ttu-id="5a887-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="5a887-169">The more information Url.</span></span> <span data-ttu-id="5a887-170">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5a887-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5a887-171">owner</span><span class="sxs-lookup"><span data-stu-id="5a887-171">owner</span></span>|<span data-ttu-id="5a887-172">Строка</span><span class="sxs-lookup"><span data-stu-id="5a887-172">String</span></span>|<span data-ttu-id="5a887-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="5a887-173">The owner of the app.</span></span> <span data-ttu-id="5a887-174">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5a887-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5a887-175">developer</span><span class="sxs-lookup"><span data-stu-id="5a887-175">developer</span></span>|<span data-ttu-id="5a887-176">String</span><span class="sxs-lookup"><span data-stu-id="5a887-176">String</span></span>|<span data-ttu-id="5a887-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="5a887-177">The developer of the app.</span></span> <span data-ttu-id="5a887-178">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5a887-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5a887-179">notes</span><span class="sxs-lookup"><span data-stu-id="5a887-179">notes</span></span>|<span data-ttu-id="5a887-180">String</span><span class="sxs-lookup"><span data-stu-id="5a887-180">String</span></span>|<span data-ttu-id="5a887-181">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="5a887-181">Notes for the app.</span></span> <span data-ttu-id="5a887-182">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5a887-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5a887-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="5a887-183">uploadState</span></span>|<span data-ttu-id="5a887-184">Int32</span><span class="sxs-lookup"><span data-stu-id="5a887-184">Int32</span></span>|<span data-ttu-id="5a887-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="5a887-185">The upload state.</span></span> <span data-ttu-id="5a887-186">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5a887-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5a887-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="5a887-187">publishingState</span></span>|[<span data-ttu-id="5a887-188">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="5a887-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="5a887-189">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="5a887-189">The publishing state for the app.</span></span> <span data-ttu-id="5a887-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="5a887-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="5a887-191">НаСледуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5a887-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="5a887-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="5a887-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="5a887-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="5a887-193">isAssigned</span></span>|<span data-ttu-id="5a887-194">Логический</span><span class="sxs-lookup"><span data-stu-id="5a887-194">Boolean</span></span>|<span data-ttu-id="5a887-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="5a887-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="5a887-196">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5a887-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5a887-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5a887-197">roleScopeTagIds</span></span>|<span data-ttu-id="5a887-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="5a887-198">String collection</span></span>|<span data-ttu-id="5a887-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="5a887-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="5a887-200">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5a887-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5a887-201">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="5a887-201">committedContentVersion</span></span>|<span data-ttu-id="5a887-202">String</span><span class="sxs-lookup"><span data-stu-id="5a887-202">String</span></span>|<span data-ttu-id="5a887-203">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="5a887-203">The internal committed content version.</span></span> <span data-ttu-id="5a887-204">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="5a887-204">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="5a887-205">fileName</span><span class="sxs-lookup"><span data-stu-id="5a887-205">fileName</span></span>|<span data-ttu-id="5a887-206">String</span><span class="sxs-lookup"><span data-stu-id="5a887-206">String</span></span>|<span data-ttu-id="5a887-207">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="5a887-207">The name of the main Lob application file.</span></span> <span data-ttu-id="5a887-208">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="5a887-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="5a887-209">size</span><span class="sxs-lookup"><span data-stu-id="5a887-209">size</span></span>|<span data-ttu-id="5a887-210">Int64</span><span class="sxs-lookup"><span data-stu-id="5a887-210">Int64</span></span>|<span data-ttu-id="5a887-211">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="5a887-211">The total size, including all uploaded files.</span></span> <span data-ttu-id="5a887-212">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="5a887-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="5a887-213">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="5a887-213">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="5a887-214">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="5a887-214">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="5a887-215">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="5a887-215">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="5a887-216">Продуктидентифиер</span><span class="sxs-lookup"><span data-stu-id="5a887-216">productIdentifier</span></span>|<span data-ttu-id="5a887-217">String</span><span class="sxs-lookup"><span data-stu-id="5a887-217">String</span></span>|<span data-ttu-id="5a887-218">Идентификатор продукта.</span><span class="sxs-lookup"><span data-stu-id="5a887-218">The Product Identifier.</span></span>|
|<span data-ttu-id="5a887-219">identityVersion</span><span class="sxs-lookup"><span data-stu-id="5a887-219">identityVersion</span></span>|<span data-ttu-id="5a887-220">String</span><span class="sxs-lookup"><span data-stu-id="5a887-220">String</span></span>|<span data-ttu-id="5a887-221">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="5a887-221">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="5a887-222">Ответ</span><span class="sxs-lookup"><span data-stu-id="5a887-222">Response</span></span>
<span data-ttu-id="5a887-223">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсфонексап](../resources/intune-apps-windowsphonexap.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5a887-223">If successful, this method returns a `200 OK` response code and an updated [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a887-224">Пример</span><span class="sxs-lookup"><span data-stu-id="5a887-224">Example</span></span>

### <a name="request"></a><span data-ttu-id="5a887-225">Запрос</span><span class="sxs-lookup"><span data-stu-id="5a887-225">Request</span></span>
<span data-ttu-id="5a887-226">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5a887-226">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1164

{
  "@odata.type": "#microsoft.graph.windowsPhoneXAP",
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
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "productIdentifier": "Product Identifier value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="5a887-227">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a887-227">Response</span></span>
<span data-ttu-id="5a887-p121">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5a887-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1336

{
  "@odata.type": "#microsoft.graph.windowsPhoneXAP",
  "id": "301ddc77-dc77-301d-77dc-1d3077dc1d30",
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
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "productIdentifier": "Product Identifier value",
  "identityVersion": "Identity Version value"
}
```




