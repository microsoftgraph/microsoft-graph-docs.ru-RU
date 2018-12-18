---
title: Список managementConditions
description: Свойства списка и связей объектов managementCondition.
author: tfitzmac
ms.openlocfilehash: 1a0ee53cf36569df8603d933f143713634e4b436
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344585"
---
# <a name="list-managementconditions"></a><span data-ttu-id="1d1c2-103">Список managementConditions</span><span class="sxs-lookup"><span data-stu-id="1d1c2-103">List managementConditions</span></span>

> <span data-ttu-id="1d1c2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1d1c2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1d1c2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d1c2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1d1c2-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1d1c2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1d1c2-107">Свойства списка и связей объектов [managementCondition](../resources/intune-fencing-managementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="1d1c2-107">List properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1d1c2-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1d1c2-108">Prerequisites</span></span>
<span data-ttu-id="1d1c2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d1c2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d1c2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1d1c2-111">Permission type</span></span>|<span data-ttu-id="1d1c2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1d1c2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d1c2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1d1c2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1d1c2-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1d1c2-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1d1c2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1d1c2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d1c2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d1c2-116">Not supported.</span></span>|
|<span data-ttu-id="1d1c2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1d1c2-117">Application</span></span>|<span data-ttu-id="1d1c2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d1c2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d1c2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1d1c2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="1d1c2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1d1c2-120">Request headers</span></span>
|<span data-ttu-id="1d1c2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1d1c2-121">Header</span></span>|<span data-ttu-id="1d1c2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1d1c2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d1c2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1d1c2-123">Authorization</span></span>|<span data-ttu-id="1d1c2-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1d1c2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d1c2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1d1c2-125">Accept</span></span>|<span data-ttu-id="1d1c2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1d1c2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d1c2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1d1c2-127">Request body</span></span>
<span data-ttu-id="1d1c2-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1d1c2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d1c2-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="1d1c2-129">Response</span></span>
<span data-ttu-id="1d1c2-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [managementCondition](../resources/intune-fencing-managementcondition.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1d1c2-130">If successful, this method returns a `200 OK` response code and a collection of [managementCondition](../resources/intune-fencing-managementcondition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d1c2-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1d1c2-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="1d1c2-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1d1c2-132">Request</span></span>
<span data-ttu-id="1d1c2-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1d1c2-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions
```

### <a name="response"></a><span data-ttu-id="1d1c2-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="1d1c2-134">Response</span></span>
<span data-ttu-id="1d1c2-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1d1c2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 504

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managementCondition",
      "id": "5cb49381-9381-5cb4-8193-b45c8193b45c",
      "uniqueName": "Unique Name value",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
      "eTag": "ETag value",
      "applicablePlatforms": [
        "androidForWork"
      ]
    }
  ]
}
```





