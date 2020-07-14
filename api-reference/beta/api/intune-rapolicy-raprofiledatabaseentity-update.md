---
title: Обновление Рапрофиледатабасинтити
description: Обновление свойств объекта Рапрофиледатабасинтити.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 232ba8a54548f3d9fd702f65b2d459d6d97c4f3c
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45124343"
---
# <a name="update-raprofiledatabaseentity"></a><span data-ttu-id="de1b8-103">Обновление Рапрофиледатабасинтити</span><span class="sxs-lookup"><span data-stu-id="de1b8-103">Update raProfileDatabaseEntity</span></span>

<span data-ttu-id="de1b8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de1b8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="de1b8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de1b8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de1b8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="de1b8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de1b8-107">Обновление свойств объекта [рапрофиледатабасинтити](../resources/intune-rapolicy-raprofiledatabaseentity.md) .</span><span class="sxs-lookup"><span data-stu-id="de1b8-107">Update the properties of a [raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="de1b8-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="de1b8-108">Prerequisites</span></span>
<span data-ttu-id="de1b8-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="de1b8-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="de1b8-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de1b8-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de1b8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de1b8-111">Permission type</span></span>|<span data-ttu-id="de1b8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="de1b8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de1b8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de1b8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="de1b8-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de1b8-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="de1b8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de1b8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de1b8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de1b8-116">Not supported.</span></span>|
|<span data-ttu-id="de1b8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="de1b8-117">Application</span></span>|<span data-ttu-id="de1b8-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de1b8-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="de1b8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de1b8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /resourceAccessProfileEntities/{resourceAccessProfileEntitiesId}
```

## <a name="request-headers"></a><span data-ttu-id="de1b8-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="de1b8-120">Request headers</span></span>
|<span data-ttu-id="de1b8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="de1b8-121">Header</span></span>|<span data-ttu-id="de1b8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="de1b8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de1b8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="de1b8-123">Authorization</span></span>|<span data-ttu-id="de1b8-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de1b8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de1b8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="de1b8-125">Accept</span></span>|<span data-ttu-id="de1b8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="de1b8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de1b8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="de1b8-127">Request body</span></span>
<span data-ttu-id="de1b8-128">В тексте запроса добавьте представление объекта [рапрофиледатабасинтити](../resources/intune-rapolicy-raprofiledatabaseentity.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="de1b8-128">In the request body, supply a JSON representation for the [raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md) object.</span></span>

<span data-ttu-id="de1b8-129">В следующей таблице приведены свойства, необходимые при создании [рапрофиледатабасинтити](../resources/intune-rapolicy-raprofiledatabaseentity.md).</span><span class="sxs-lookup"><span data-stu-id="de1b8-129">The following table shows the properties that are required when you create the [raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md).</span></span>

|<span data-ttu-id="de1b8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="de1b8-130">Property</span></span>|<span data-ttu-id="de1b8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="de1b8-131">Type</span></span>|<span data-ttu-id="de1b8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="de1b8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de1b8-133">version</span><span class="sxs-lookup"><span data-stu-id="de1b8-133">version</span></span>|<span data-ttu-id="de1b8-134">Int32</span><span class="sxs-lookup"><span data-stu-id="de1b8-134">Int32</span></span>|<span data-ttu-id="de1b8-135">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="de1b8-135">Not yet documented</span></span>|
|<span data-ttu-id="de1b8-136">isDeleted</span><span class="sxs-lookup"><span data-stu-id="de1b8-136">isDeleted</span></span>|<span data-ttu-id="de1b8-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="de1b8-137">Boolean</span></span>|<span data-ttu-id="de1b8-138">Пока не задокументировано</span><span class="sxs-lookup"><span data-stu-id="de1b8-138">Not yet documented</span></span>|
|<span data-ttu-id="de1b8-139">софтделетедтиме</span><span class="sxs-lookup"><span data-stu-id="de1b8-139">softDeletedTime</span></span>|<span data-ttu-id="de1b8-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de1b8-140">DateTimeOffset</span></span>|<span data-ttu-id="de1b8-141">Н/Д</span><span class="sxs-lookup"><span data-stu-id="de1b8-141">Not yet documented</span></span>|
|<span data-ttu-id="de1b8-142">displayName</span><span class="sxs-lookup"><span data-stu-id="de1b8-142">displayName</span></span>|<span data-ttu-id="de1b8-143">Строка</span><span class="sxs-lookup"><span data-stu-id="de1b8-143">String</span></span>|<span data-ttu-id="de1b8-144">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="de1b8-144">Not yet documented</span></span>|
|<span data-ttu-id="de1b8-145">линкедпрофилеидс</span><span class="sxs-lookup"><span data-stu-id="de1b8-145">linkedProfileIds</span></span>|<span data-ttu-id="de1b8-146">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="de1b8-146">Guid collection</span></span>|<span data-ttu-id="de1b8-147">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="de1b8-147">Not yet documented</span></span>|
|<span data-ttu-id="de1b8-148">профилетипенаме</span><span class="sxs-lookup"><span data-stu-id="de1b8-148">profileTypeName</span></span>|<span data-ttu-id="de1b8-149">String</span><span class="sxs-lookup"><span data-stu-id="de1b8-149">String</span></span>|<span data-ttu-id="de1b8-150">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="de1b8-150">Not yet documented</span></span>|
|<span data-ttu-id="de1b8-151">профилебоди</span><span class="sxs-lookup"><span data-stu-id="de1b8-151">profileBody</span></span>|<span data-ttu-id="de1b8-152">String</span><span class="sxs-lookup"><span data-stu-id="de1b8-152">String</span></span>|<span data-ttu-id="de1b8-153">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="de1b8-153">Not yet documented</span></span>|
|<span data-ttu-id="de1b8-154">профилебодихаш</span><span class="sxs-lookup"><span data-stu-id="de1b8-154">profileBodyHash</span></span>|<span data-ttu-id="de1b8-155">String</span><span class="sxs-lookup"><span data-stu-id="de1b8-155">String</span></span>|<span data-ttu-id="de1b8-156">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="de1b8-156">Not yet documented</span></span>|
|<span data-ttu-id="de1b8-157">platformType</span><span class="sxs-lookup"><span data-stu-id="de1b8-157">platformType</span></span>|<span data-ttu-id="de1b8-158">Int32</span><span class="sxs-lookup"><span data-stu-id="de1b8-158">Int32</span></span>|<span data-ttu-id="de1b8-159">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="de1b8-159">Not yet documented</span></span>|
|<span data-ttu-id="de1b8-160">трансформедпрофилебоди</span><span class="sxs-lookup"><span data-stu-id="de1b8-160">transformedProfileBody</span></span>|<span data-ttu-id="de1b8-161">String</span><span class="sxs-lookup"><span data-stu-id="de1b8-161">String</span></span>|<span data-ttu-id="de1b8-162">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="de1b8-162">Not yet documented</span></span>|
|<span data-ttu-id="de1b8-163">трансформедпрофилебодихаш</span><span class="sxs-lookup"><span data-stu-id="de1b8-163">transformedProfileBodyHash</span></span>|<span data-ttu-id="de1b8-164">String</span><span class="sxs-lookup"><span data-stu-id="de1b8-164">String</span></span>|<span data-ttu-id="de1b8-165">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="de1b8-165">Not yet documented</span></span>|
|<span data-ttu-id="de1b8-166">tenantId</span><span class="sxs-lookup"><span data-stu-id="de1b8-166">tenantId</span></span>|<span data-ttu-id="de1b8-167">Guid</span><span class="sxs-lookup"><span data-stu-id="de1b8-167">Guid</span></span>|<span data-ttu-id="de1b8-168">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="de1b8-168">Not yet documented</span></span>|
|<span data-ttu-id="de1b8-169">профилеид</span><span class="sxs-lookup"><span data-stu-id="de1b8-169">profileId</span></span>|<span data-ttu-id="de1b8-170">Guid</span><span class="sxs-lookup"><span data-stu-id="de1b8-170">Guid</span></span>|<span data-ttu-id="de1b8-171">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="de1b8-171">Not yet documented</span></span>|
|<span data-ttu-id="de1b8-172">eTag</span><span class="sxs-lookup"><span data-stu-id="de1b8-172">eTag</span></span>|<span data-ttu-id="de1b8-173">String</span><span class="sxs-lookup"><span data-stu-id="de1b8-173">String</span></span>|<span data-ttu-id="de1b8-174">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="de1b8-174">Not yet documented</span></span>|
|<span data-ttu-id="de1b8-175">Схемы</span><span class="sxs-lookup"><span data-stu-id="de1b8-175">schemaVersion</span></span>|[<span data-ttu-id="de1b8-176">раполицисервицеверсионс</span><span class="sxs-lookup"><span data-stu-id="de1b8-176">raPolicyServiceVersions</span></span>](../resources/intune-rapolicy-rapolicyserviceversions.md)|<span data-ttu-id="de1b8-177">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="de1b8-177">Not yet documented.</span></span> <span data-ttu-id="de1b8-178">Возможные значения: `initial`, `betaStart`, `experimentStart`, `mmpcStart`, `iosStart`.</span><span class="sxs-lookup"><span data-stu-id="de1b8-178">Possible values are: `initial`, `betaStart`, `experimentStart`, `mmpcStart`, `iosStart`.</span></span>|
|<span data-ttu-id="de1b8-179">Дата</span><span class="sxs-lookup"><span data-stu-id="de1b8-179">lastModified</span></span>|<span data-ttu-id="de1b8-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de1b8-180">DateTimeOffset</span></span>|<span data-ttu-id="de1b8-181">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="de1b8-181">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="de1b8-182">Ответ</span><span class="sxs-lookup"><span data-stu-id="de1b8-182">Response</span></span>
<span data-ttu-id="de1b8-183">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [рапрофиледатабасинтити](../resources/intune-rapolicy-raprofiledatabaseentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="de1b8-183">If successful, this method returns a `200 OK` response code and an updated [raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de1b8-184">Пример</span><span class="sxs-lookup"><span data-stu-id="de1b8-184">Example</span></span>

### <a name="request"></a><span data-ttu-id="de1b8-185">Запрос</span><span class="sxs-lookup"><span data-stu-id="de1b8-185">Request</span></span>
<span data-ttu-id="de1b8-186">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="de1b8-186">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/resourceAccessProfileEntities/{resourceAccessProfileEntitiesId}
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

### <a name="response"></a><span data-ttu-id="de1b8-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="de1b8-187">Response</span></span>
<span data-ttu-id="de1b8-188">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="de1b8-188">Here is an example of the response.</span></span> <span data-ttu-id="de1b8-189">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="de1b8-189">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="de1b8-190">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="de1b8-190">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



