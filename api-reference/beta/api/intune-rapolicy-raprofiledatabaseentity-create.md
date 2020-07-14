---
title: Создание Рапрофиледатабасинтити
description: Создание нового объекта Рапрофиледатабасинтити.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cb892f1a64dd1223956f3fda73a6aeb8512edf00
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45124362"
---
# <a name="create-raprofiledatabaseentity"></a><span data-ttu-id="3f1b9-103">Создание Рапрофиледатабасинтити</span><span class="sxs-lookup"><span data-stu-id="3f1b9-103">Create raProfileDatabaseEntity</span></span>

<span data-ttu-id="3f1b9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f1b9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3f1b9-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f1b9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f1b9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3f1b9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f1b9-107">Создание нового объекта [рапрофиледатабасинтити](../resources/intune-rapolicy-raprofiledatabaseentity.md) .</span><span class="sxs-lookup"><span data-stu-id="3f1b9-107">Create a new [raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3f1b9-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3f1b9-108">Prerequisites</span></span>
<span data-ttu-id="3f1b9-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="3f1b9-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="3f1b9-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f1b9-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f1b9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3f1b9-111">Permission type</span></span>|<span data-ttu-id="3f1b9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3f1b9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3f1b9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3f1b9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3f1b9-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f1b9-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3f1b9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3f1b9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3f1b9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f1b9-116">Not supported.</span></span>|
|<span data-ttu-id="3f1b9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3f1b9-117">Application</span></span>|<span data-ttu-id="3f1b9-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f1b9-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3f1b9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3f1b9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /resourceAccessProfileEntities
```

## <a name="request-headers"></a><span data-ttu-id="3f1b9-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3f1b9-120">Request headers</span></span>
|<span data-ttu-id="3f1b9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3f1b9-121">Header</span></span>|<span data-ttu-id="3f1b9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3f1b9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3f1b9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3f1b9-123">Authorization</span></span>|<span data-ttu-id="3f1b9-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3f1b9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3f1b9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3f1b9-125">Accept</span></span>|<span data-ttu-id="3f1b9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3f1b9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f1b9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3f1b9-127">Request body</span></span>
<span data-ttu-id="3f1b9-128">В тексте запроса добавьте представление объекта Рапрофиледатабасинтити в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3f1b9-128">In the request body, supply a JSON representation for the raProfileDatabaseEntity object.</span></span>

<span data-ttu-id="3f1b9-129">В следующей таблице приведены свойства, необходимые при создании Рапрофиледатабасинтити.</span><span class="sxs-lookup"><span data-stu-id="3f1b9-129">The following table shows the properties that are required when you create the raProfileDatabaseEntity.</span></span>

|<span data-ttu-id="3f1b9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3f1b9-130">Property</span></span>|<span data-ttu-id="3f1b9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3f1b9-131">Type</span></span>|<span data-ttu-id="3f1b9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3f1b9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f1b9-133">version</span><span class="sxs-lookup"><span data-stu-id="3f1b9-133">version</span></span>|<span data-ttu-id="3f1b9-134">Int32</span><span class="sxs-lookup"><span data-stu-id="3f1b9-134">Int32</span></span>|<span data-ttu-id="3f1b9-135">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="3f1b9-135">Not yet documented</span></span>|
|<span data-ttu-id="3f1b9-136">isDeleted</span><span class="sxs-lookup"><span data-stu-id="3f1b9-136">isDeleted</span></span>|<span data-ttu-id="3f1b9-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f1b9-137">Boolean</span></span>|<span data-ttu-id="3f1b9-138">Пока не задокументировано</span><span class="sxs-lookup"><span data-stu-id="3f1b9-138">Not yet documented</span></span>|
|<span data-ttu-id="3f1b9-139">софтделетедтиме</span><span class="sxs-lookup"><span data-stu-id="3f1b9-139">softDeletedTime</span></span>|<span data-ttu-id="3f1b9-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f1b9-140">DateTimeOffset</span></span>|<span data-ttu-id="3f1b9-141">Н/Д</span><span class="sxs-lookup"><span data-stu-id="3f1b9-141">Not yet documented</span></span>|
|<span data-ttu-id="3f1b9-142">displayName</span><span class="sxs-lookup"><span data-stu-id="3f1b9-142">displayName</span></span>|<span data-ttu-id="3f1b9-143">Строка</span><span class="sxs-lookup"><span data-stu-id="3f1b9-143">String</span></span>|<span data-ttu-id="3f1b9-144">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="3f1b9-144">Not yet documented</span></span>|
|<span data-ttu-id="3f1b9-145">линкедпрофилеидс</span><span class="sxs-lookup"><span data-stu-id="3f1b9-145">linkedProfileIds</span></span>|<span data-ttu-id="3f1b9-146">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="3f1b9-146">Guid collection</span></span>|<span data-ttu-id="3f1b9-147">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="3f1b9-147">Not yet documented</span></span>|
|<span data-ttu-id="3f1b9-148">профилетипенаме</span><span class="sxs-lookup"><span data-stu-id="3f1b9-148">profileTypeName</span></span>|<span data-ttu-id="3f1b9-149">String</span><span class="sxs-lookup"><span data-stu-id="3f1b9-149">String</span></span>|<span data-ttu-id="3f1b9-150">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="3f1b9-150">Not yet documented</span></span>|
|<span data-ttu-id="3f1b9-151">профилебоди</span><span class="sxs-lookup"><span data-stu-id="3f1b9-151">profileBody</span></span>|<span data-ttu-id="3f1b9-152">String</span><span class="sxs-lookup"><span data-stu-id="3f1b9-152">String</span></span>|<span data-ttu-id="3f1b9-153">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="3f1b9-153">Not yet documented</span></span>|
|<span data-ttu-id="3f1b9-154">профилебодихаш</span><span class="sxs-lookup"><span data-stu-id="3f1b9-154">profileBodyHash</span></span>|<span data-ttu-id="3f1b9-155">String</span><span class="sxs-lookup"><span data-stu-id="3f1b9-155">String</span></span>|<span data-ttu-id="3f1b9-156">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="3f1b9-156">Not yet documented</span></span>|
|<span data-ttu-id="3f1b9-157">platformType</span><span class="sxs-lookup"><span data-stu-id="3f1b9-157">platformType</span></span>|<span data-ttu-id="3f1b9-158">Int32</span><span class="sxs-lookup"><span data-stu-id="3f1b9-158">Int32</span></span>|<span data-ttu-id="3f1b9-159">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="3f1b9-159">Not yet documented</span></span>|
|<span data-ttu-id="3f1b9-160">трансформедпрофилебоди</span><span class="sxs-lookup"><span data-stu-id="3f1b9-160">transformedProfileBody</span></span>|<span data-ttu-id="3f1b9-161">String</span><span class="sxs-lookup"><span data-stu-id="3f1b9-161">String</span></span>|<span data-ttu-id="3f1b9-162">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="3f1b9-162">Not yet documented</span></span>|
|<span data-ttu-id="3f1b9-163">трансформедпрофилебодихаш</span><span class="sxs-lookup"><span data-stu-id="3f1b9-163">transformedProfileBodyHash</span></span>|<span data-ttu-id="3f1b9-164">String</span><span class="sxs-lookup"><span data-stu-id="3f1b9-164">String</span></span>|<span data-ttu-id="3f1b9-165">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="3f1b9-165">Not yet documented</span></span>|
|<span data-ttu-id="3f1b9-166">tenantId</span><span class="sxs-lookup"><span data-stu-id="3f1b9-166">tenantId</span></span>|<span data-ttu-id="3f1b9-167">Guid</span><span class="sxs-lookup"><span data-stu-id="3f1b9-167">Guid</span></span>|<span data-ttu-id="3f1b9-168">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="3f1b9-168">Not yet documented</span></span>|
|<span data-ttu-id="3f1b9-169">профилеид</span><span class="sxs-lookup"><span data-stu-id="3f1b9-169">profileId</span></span>|<span data-ttu-id="3f1b9-170">Guid</span><span class="sxs-lookup"><span data-stu-id="3f1b9-170">Guid</span></span>|<span data-ttu-id="3f1b9-171">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="3f1b9-171">Not yet documented</span></span>|
|<span data-ttu-id="3f1b9-172">eTag</span><span class="sxs-lookup"><span data-stu-id="3f1b9-172">eTag</span></span>|<span data-ttu-id="3f1b9-173">String</span><span class="sxs-lookup"><span data-stu-id="3f1b9-173">String</span></span>|<span data-ttu-id="3f1b9-174">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="3f1b9-174">Not yet documented</span></span>|
|<span data-ttu-id="3f1b9-175">Схемы</span><span class="sxs-lookup"><span data-stu-id="3f1b9-175">schemaVersion</span></span>|[<span data-ttu-id="3f1b9-176">раполицисервицеверсионс</span><span class="sxs-lookup"><span data-stu-id="3f1b9-176">raPolicyServiceVersions</span></span>](../resources/intune-rapolicy-rapolicyserviceversions.md)|<span data-ttu-id="3f1b9-177">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="3f1b9-177">Not yet documented.</span></span> <span data-ttu-id="3f1b9-178">Возможные значения: `initial`, `betaStart`, `experimentStart`, `mmpcStart`, `iosStart`.</span><span class="sxs-lookup"><span data-stu-id="3f1b9-178">Possible values are: `initial`, `betaStart`, `experimentStart`, `mmpcStart`, `iosStart`.</span></span>|
|<span data-ttu-id="3f1b9-179">Дата</span><span class="sxs-lookup"><span data-stu-id="3f1b9-179">lastModified</span></span>|<span data-ttu-id="3f1b9-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f1b9-180">DateTimeOffset</span></span>|<span data-ttu-id="3f1b9-181">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="3f1b9-181">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3f1b9-182">Ответ</span><span class="sxs-lookup"><span data-stu-id="3f1b9-182">Response</span></span>
<span data-ttu-id="3f1b9-183">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [рапрофиледатабасинтити](../resources/intune-rapolicy-raprofiledatabaseentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3f1b9-183">If successful, this method returns a `201 Created` response code and a [raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f1b9-184">Пример</span><span class="sxs-lookup"><span data-stu-id="3f1b9-184">Example</span></span>

### <a name="request"></a><span data-ttu-id="3f1b9-185">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f1b9-185">Request</span></span>
<span data-ttu-id="3f1b9-186">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3f1b9-186">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/resourceAccessProfileEntities
Content-type: application/json
Content-length: 799

{
  "@odata.type": "#microsoft.graph.raProfileDatabaseEntity",
  "version": 7,
  "isDeleted": true,
  "softDeletedTime": "2016-12-31T23:59:22.6041454-08:00",
  "displayName": "Display Name value",
  "linkedProfileIds": [
    "5b59ac1a-ac1a-5b59-1aac-595b1aac595b"
  ],
  "profileTypeName": "Profile Type Name value",
  "profileBody": "Profile Body value",
  "profileBodyHash": "Profile Body Hash value",
  "platformType": 12,
  "transformedProfileBody": "Transformed Profile Body value",
  "transformedProfileBodyHash": "Transformed Profile Body Hash value",
  "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
  "profileId": "6389d896-d896-6389-96d8-896396d88963",
  "eTag": "ETag value",
  "schemaVersion": "betaStart",
  "lastModified": "2017-01-01T00:03:14.6651031-08:00"
}
```

### <a name="response"></a><span data-ttu-id="3f1b9-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f1b9-187">Response</span></span>
<span data-ttu-id="3f1b9-188">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="3f1b9-188">Here is an example of the response.</span></span> <span data-ttu-id="3f1b9-189">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="3f1b9-189">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3f1b9-190">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="3f1b9-190">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 799

{
  "@odata.type": "#microsoft.graph.raProfileDatabaseEntity",
  "version": 7,
  "isDeleted": true,
  "softDeletedTime": "2016-12-31T23:59:22.6041454-08:00",
  "displayName": "Display Name value",
  "linkedProfileIds": [
    "5b59ac1a-ac1a-5b59-1aac-595b1aac595b"
  ],
  "profileTypeName": "Profile Type Name value",
  "profileBody": "Profile Body value",
  "profileBodyHash": "Profile Body Hash value",
  "platformType": 12,
  "transformedProfileBody": "Transformed Profile Body value",
  "transformedProfileBodyHash": "Transformed Profile Body Hash value",
  "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
  "profileId": "6389d896-d896-6389-96d8-896396d88963",
  "eTag": "ETag value",
  "schemaVersion": "betaStart",
  "lastModified": "2017-01-01T00:03:14.6651031-08:00"
}
```



