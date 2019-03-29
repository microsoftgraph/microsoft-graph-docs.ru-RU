---
title: Перечисление объектов notificationMessageTemplate
description: Список свойств и связей объектов notificationMessageTemplate.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3c5b342be039b6ae5bf9d0ce0e5a49720070b239
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30972601"
---
# <a name="list-notificationmessagetemplates"></a><span data-ttu-id="10f1d-103">Перечисление объектов notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="10f1d-103">List notificationMessageTemplates</span></span>

> <span data-ttu-id="10f1d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10f1d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10f1d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="10f1d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10f1d-106">Список свойств и связей объектов [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="10f1d-106">List properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="10f1d-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="10f1d-107">Prerequisites</span></span>
<span data-ttu-id="10f1d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10f1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10f1d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10f1d-110">Permission type</span></span>|<span data-ttu-id="10f1d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="10f1d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10f1d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10f1d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="10f1d-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="10f1d-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="10f1d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10f1d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10f1d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10f1d-115">Not supported.</span></span>|
|<span data-ttu-id="10f1d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="10f1d-116">Application</span></span>|<span data-ttu-id="10f1d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10f1d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="10f1d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10f1d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/notificationMessageTemplates
```

## <a name="request-headers"></a><span data-ttu-id="10f1d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10f1d-119">Request headers</span></span>
|<span data-ttu-id="10f1d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="10f1d-120">Header</span></span>|<span data-ttu-id="10f1d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="10f1d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10f1d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="10f1d-122">Authorization</span></span>|<span data-ttu-id="10f1d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10f1d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10f1d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="10f1d-124">Accept</span></span>|<span data-ttu-id="10f1d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="10f1d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10f1d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="10f1d-126">Request body</span></span>
<span data-ttu-id="10f1d-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="10f1d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10f1d-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="10f1d-128">Response</span></span>
<span data-ttu-id="10f1d-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="10f1d-129">If successful, this method returns a `200 OK` response code and a collection of [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10f1d-130">Пример</span><span class="sxs-lookup"><span data-stu-id="10f1d-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="10f1d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="10f1d-131">Request</span></span>
<span data-ttu-id="10f1d-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10f1d-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates
```

### <a name="response"></a><span data-ttu-id="10f1d-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="10f1d-133">Response</span></span>
<span data-ttu-id="10f1d-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="10f1d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 441

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.notificationMessageTemplate",
      "id": "e1db399b-399b-e1db-9b39-dbe19b39dbe1",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "defaultLocale": "Default Locale value",
      "brandingOptions": "includeCompanyLogo",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ]
    }
  ]
}
```




