---
title: Список Виндовсмикрософтеджеаппс
description: Список свойств и связей объектов Виндовсмикрософтеджеапп.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5482a229d156d6ed3655c5c18c49f0767ef132dd
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43403738"
---
# <a name="list-windowsmicrosoftedgeapps"></a><span data-ttu-id="ba2d2-103">Список Виндовсмикрософтеджеаппс</span><span class="sxs-lookup"><span data-stu-id="ba2d2-103">List windowsMicrosoftEdgeApps</span></span>

<span data-ttu-id="ba2d2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba2d2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ba2d2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba2d2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba2d2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ba2d2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba2d2-107">Список свойств и связей объектов [виндовсмикрософтеджеапп](../resources/intune-apps-windowsmicrosoftedgeapp.md) .</span><span class="sxs-lookup"><span data-stu-id="ba2d2-107">List properties and relationships of the [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ba2d2-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ba2d2-108">Prerequisites</span></span>
<span data-ttu-id="ba2d2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba2d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba2d2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba2d2-111">Permission type</span></span>|<span data-ttu-id="ba2d2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba2d2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba2d2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba2d2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ba2d2-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ba2d2-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ba2d2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba2d2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba2d2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba2d2-116">Not supported.</span></span>|
|<span data-ttu-id="ba2d2-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="ba2d2-117">Application</span></span>|<span data-ttu-id="ba2d2-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ba2d2-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba2d2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba2d2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="ba2d2-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ba2d2-120">Request headers</span></span>
|<span data-ttu-id="ba2d2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ba2d2-121">Header</span></span>|<span data-ttu-id="ba2d2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ba2d2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba2d2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba2d2-123">Authorization</span></span>|<span data-ttu-id="ba2d2-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ba2d2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba2d2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ba2d2-125">Accept</span></span>|<span data-ttu-id="ba2d2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ba2d2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba2d2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ba2d2-127">Request body</span></span>
<span data-ttu-id="ba2d2-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ba2d2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba2d2-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="ba2d2-129">Response</span></span>
<span data-ttu-id="ba2d2-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [виндовсмикрософтеджеапп](../resources/intune-apps-windowsmicrosoftedgeapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ba2d2-130">If successful, this method returns a `200 OK` response code and a collection of [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba2d2-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ba2d2-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ba2d2-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba2d2-132">Request</span></span>
<span data-ttu-id="ba2d2-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ba2d2-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="ba2d2-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba2d2-134">Response</span></span>
<span data-ttu-id="ba2d2-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ba2d2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1118

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsMicrosoftEdgeApp",
      "id": "a4d4a316-a316-a4d4-16a3-d4a416a3d4a4",
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
      "dependentAppCount": 1,
      "channel": "beta",
      "displayLanguageLocale": "Display Language Locale value"
    }
  ]
}
```



