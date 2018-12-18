---
title: Список roleScopeTags
description: Свойства списка и связей объектов roleScopeTag.
author: tfitzmac
ms.openlocfilehash: 786276f5e0d74871ebf38fce235f584911bebb20
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337802"
---
# <a name="list-rolescopetags"></a><span data-ttu-id="b6ec4-103">Список roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="b6ec4-103">List roleScopeTags</span></span>

> <span data-ttu-id="b6ec4-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b6ec4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b6ec4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6ec4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b6ec4-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b6ec4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b6ec4-107">Свойства списка и связей объектов [roleScopeTag](../resources/intune-rbac-rolescopetag.md) .</span><span class="sxs-lookup"><span data-stu-id="b6ec4-107">List properties and relationships of the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b6ec4-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b6ec4-108">Prerequisites</span></span>
<span data-ttu-id="b6ec4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6ec4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6ec4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b6ec4-111">Permission type</span></span>|<span data-ttu-id="b6ec4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b6ec4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6ec4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b6ec4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b6ec4-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6ec4-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="b6ec4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b6ec4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6ec4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6ec4-116">Not supported.</span></span>|
|<span data-ttu-id="b6ec4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b6ec4-117">Application</span></span>|<span data-ttu-id="b6ec4-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6ec4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6ec4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b6ec4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleScopeTags
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags
```

## <a name="request-headers"></a><span data-ttu-id="b6ec4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b6ec4-120">Request headers</span></span>
|<span data-ttu-id="b6ec4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b6ec4-121">Header</span></span>|<span data-ttu-id="b6ec4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b6ec4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6ec4-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b6ec4-123">Authorization</span></span>|<span data-ttu-id="b6ec4-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b6ec4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6ec4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b6ec4-125">Accept</span></span>|<span data-ttu-id="b6ec4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b6ec4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6ec4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b6ec4-127">Request body</span></span>
<span data-ttu-id="b6ec4-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b6ec4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6ec4-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="b6ec4-129">Response</span></span>
<span data-ttu-id="b6ec4-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [roleScopeTag](../resources/intune-rbac-rolescopetag.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b6ec4-130">If successful, this method returns a `200 OK` response code and a collection of [roleScopeTag](../resources/intune-rbac-rolescopetag.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6ec4-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b6ec4-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="b6ec4-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b6ec4-132">Request</span></span>
<span data-ttu-id="b6ec4-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b6ec4-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleScopeTags
```

### <a name="response"></a><span data-ttu-id="b6ec4-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="b6ec4-134">Response</span></span>
<span data-ttu-id="b6ec4-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b6ec4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 231

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.roleScopeTag",
      "id": "9ed1e179-e179-9ed1-79e1-d19e79e1d19e",
      "displayName": "Display Name value",
      "description": "Description value"
    }
  ]
}
```





