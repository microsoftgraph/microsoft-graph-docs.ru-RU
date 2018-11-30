---
title: функция getRoleScopeTagsByResource
description: Н/Д
ms.openlocfilehash: c6ccea13ee3b3314099573cb79625e1084ffdc13
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080473"
---
# <a name="getrolescopetagsbyresource-function"></a><span data-ttu-id="43576-103">функция getRoleScopeTagsByResource</span><span class="sxs-lookup"><span data-stu-id="43576-103">getRoleScopeTagsByResource function</span></span>

> <span data-ttu-id="43576-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="43576-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="43576-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43576-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="43576-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="43576-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="43576-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="43576-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="43576-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="43576-108">Prerequisites</span></span>
<span data-ttu-id="43576-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43576-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43576-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="43576-111">Permission type</span></span>|<span data-ttu-id="43576-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="43576-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43576-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="43576-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="43576-114">&nbsp;&nbsp; **Управления доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="43576-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="43576-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="43576-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="43576-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="43576-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43576-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43576-117">Not supported.</span></span>|
|<span data-ttu-id="43576-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="43576-118">Application</span></span>|<span data-ttu-id="43576-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43576-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43576-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="43576-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getRoleScopeTagsByResource
```

## <a name="request-headers"></a><span data-ttu-id="43576-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="43576-121">Request headers</span></span>
|<span data-ttu-id="43576-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="43576-122">Header</span></span>|<span data-ttu-id="43576-123">Значение</span><span class="sxs-lookup"><span data-stu-id="43576-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43576-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="43576-124">Authorization</span></span>|<span data-ttu-id="43576-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="43576-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43576-126">Accept</span><span class="sxs-lookup"><span data-stu-id="43576-126">Accept</span></span>|<span data-ttu-id="43576-127">application/json</span><span class="sxs-lookup"><span data-stu-id="43576-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43576-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="43576-128">Request body</span></span>
<span data-ttu-id="43576-129">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="43576-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="43576-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="43576-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="43576-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="43576-131">Property</span></span>|<span data-ttu-id="43576-132">Тип</span><span class="sxs-lookup"><span data-stu-id="43576-132">Type</span></span>|<span data-ttu-id="43576-133">Описание</span><span class="sxs-lookup"><span data-stu-id="43576-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43576-134">resource</span><span class="sxs-lookup"><span data-stu-id="43576-134">resource</span></span>|<span data-ttu-id="43576-135">String</span><span class="sxs-lookup"><span data-stu-id="43576-135">String</span></span>|<span data-ttu-id="43576-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="43576-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="43576-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="43576-137">Response</span></span>
<span data-ttu-id="43576-138">Если успешно завершена, эта функция возвращает `200 OK` код ответа и семейства [roleScopeTag](../resources/intune-rbac-rolescopetag.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="43576-138">If successful, this function returns a `200 OK` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43576-139">Пример</span><span class="sxs-lookup"><span data-stu-id="43576-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="43576-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="43576-140">Request</span></span>
<span data-ttu-id="43576-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="43576-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getRoleScopeTagsByResource(resource='parameterValue')
```

### <a name="response"></a><span data-ttu-id="43576-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="43576-142">Response</span></span>
<span data-ttu-id="43576-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="43576-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



