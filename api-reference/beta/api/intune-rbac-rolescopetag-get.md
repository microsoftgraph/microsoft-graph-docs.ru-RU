---
title: Получение roleScopeTag
description: Чтение свойства и связи объекта roleScopeTag.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2a0126f4b39fbee3c154837661b368512e29ac97
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983291"
---
# <a name="get-rolescopetag"></a><span data-ttu-id="90831-103">Получение roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="90831-103">Get roleScopeTag</span></span>

> <span data-ttu-id="90831-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="90831-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="90831-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90831-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="90831-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="90831-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="90831-107">Чтение свойства и связи объекта [roleScopeTag](../resources/intune-rbac-rolescopetag.md) .</span><span class="sxs-lookup"><span data-stu-id="90831-107">Read properties and relationships of the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="90831-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="90831-108">Prerequisites</span></span>
<span data-ttu-id="90831-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90831-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90831-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90831-111">Permission type</span></span>|<span data-ttu-id="90831-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="90831-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90831-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90831-113">Delegated (work or school account)</span></span>|<span data-ttu-id="90831-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="90831-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="90831-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90831-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90831-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90831-116">Not supported.</span></span>|
|<span data-ttu-id="90831-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="90831-117">Application</span></span>|<span data-ttu-id="90831-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90831-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="90831-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90831-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleScopeTags/{roleScopeTagId}
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="90831-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="90831-120">Optional query parameters</span></span>
<span data-ttu-id="90831-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="90831-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="90831-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="90831-122">Request headers</span></span>
|<span data-ttu-id="90831-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="90831-123">Header</span></span>|<span data-ttu-id="90831-124">Значение</span><span class="sxs-lookup"><span data-stu-id="90831-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90831-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="90831-125">Authorization</span></span>|<span data-ttu-id="90831-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="90831-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90831-127">Accept</span><span class="sxs-lookup"><span data-stu-id="90831-127">Accept</span></span>|<span data-ttu-id="90831-128">application/json</span><span class="sxs-lookup"><span data-stu-id="90831-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90831-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="90831-129">Request body</span></span>
<span data-ttu-id="90831-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="90831-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90831-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="90831-131">Response</span></span>
<span data-ttu-id="90831-132">Успешно завершена, этот метод возвращает `200 OK` объект [roleScopeTag](../resources/intune-rbac-rolescopetag.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="90831-132">If successful, this method returns a `200 OK` response code and [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90831-133">Пример</span><span class="sxs-lookup"><span data-stu-id="90831-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="90831-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="90831-134">Request</span></span>
<span data-ttu-id="90831-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="90831-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleScopeTags/{roleScopeTagId}
```

### <a name="response"></a><span data-ttu-id="90831-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="90831-136">Response</span></span>
<span data-ttu-id="90831-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="90831-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 209

{
  "value": {
    "@odata.type": "#microsoft.graph.roleScopeTag",
    "id": "9ed1e179-e179-9ed1-79e1-d19e79e1d19e",
    "displayName": "Display Name value",
    "description": "Description value"
  }
}
```





