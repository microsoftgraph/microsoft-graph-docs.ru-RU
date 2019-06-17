---
title: Перечисление объектов termsAndConditions
description: Список свойств и связей объектов termsAndConditions.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 221575635da8485f37af775f41b506f7c87d8972
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34971992"
---
# <a name="list-termsandconditionses"></a><span data-ttu-id="7e921-103">Перечисление объектов termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="7e921-103">List termsAndConditionses</span></span>

> <span data-ttu-id="7e921-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e921-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e921-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7e921-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e921-106">Список свойств и связей объектов [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="7e921-106">List properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7e921-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7e921-107">Prerequisites</span></span>
<span data-ttu-id="7e921-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e921-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e921-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7e921-110">Permission type</span></span>|<span data-ttu-id="7e921-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7e921-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e921-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7e921-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7e921-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e921-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="7e921-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7e921-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e921-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e921-115">Not supported.</span></span>|
|<span data-ttu-id="7e921-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7e921-116">Application</span></span>|<span data-ttu-id="7e921-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e921-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e921-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7e921-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="7e921-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7e921-119">Request headers</span></span>
|<span data-ttu-id="7e921-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7e921-120">Header</span></span>|<span data-ttu-id="7e921-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7e921-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e921-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7e921-122">Authorization</span></span>|<span data-ttu-id="7e921-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7e921-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7e921-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7e921-124">Accept</span></span>|<span data-ttu-id="7e921-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7e921-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e921-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7e921-126">Request body</span></span>
<span data-ttu-id="7e921-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7e921-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e921-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="7e921-128">Response</span></span>
<span data-ttu-id="7e921-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7e921-129">If successful, this method returns a `200 OK` response code and a collection of [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e921-130">Пример</span><span class="sxs-lookup"><span data-stu-id="7e921-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="7e921-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e921-131">Request</span></span>
<span data-ttu-id="7e921-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7e921-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions
```

### <a name="response"></a><span data-ttu-id="7e921-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e921-133">Response</span></span>
<span data-ttu-id="7e921-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7e921-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 582

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.termsAndConditions",
      "id": "eefc80cf-80cf-eefc-cf80-fceecf80fcee",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "description": "Description value",
      "title": "Title value",
      "bodyText": "Body Text value",
      "acceptanceStatement": "Acceptance Statement value",
      "version": 7
    }
  ]
}
```





