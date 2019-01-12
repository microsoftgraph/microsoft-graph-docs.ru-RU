---
title: функция getRoleScopeTagsByResource
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d4d2b8c0b55e353e07ed60d1f8fee001f694fdc3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919780"
---
# <a name="getrolescopetagsbyresource-function"></a><span data-ttu-id="7aa21-103">функция getRoleScopeTagsByResource</span><span class="sxs-lookup"><span data-stu-id="7aa21-103">getRoleScopeTagsByResource function</span></span>

> <span data-ttu-id="7aa21-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7aa21-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7aa21-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7aa21-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7aa21-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7aa21-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7aa21-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="7aa21-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7aa21-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="7aa21-108">Prerequisites</span></span>
<span data-ttu-id="7aa21-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7aa21-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7aa21-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7aa21-111">Permission type</span></span>|<span data-ttu-id="7aa21-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7aa21-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7aa21-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7aa21-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="7aa21-114">&nbsp;&nbsp; **Управления доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="7aa21-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="7aa21-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="7aa21-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="7aa21-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7aa21-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7aa21-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7aa21-117">Not supported.</span></span>|
|<span data-ttu-id="7aa21-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7aa21-118">Application</span></span>|<span data-ttu-id="7aa21-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7aa21-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7aa21-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7aa21-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getRoleScopeTagsByResource
```

## <a name="request-headers"></a><span data-ttu-id="7aa21-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7aa21-121">Request headers</span></span>
|<span data-ttu-id="7aa21-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7aa21-122">Header</span></span>|<span data-ttu-id="7aa21-123">Значение</span><span class="sxs-lookup"><span data-stu-id="7aa21-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7aa21-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7aa21-124">Authorization</span></span>|<span data-ttu-id="7aa21-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7aa21-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7aa21-126">Accept</span><span class="sxs-lookup"><span data-stu-id="7aa21-126">Accept</span></span>|<span data-ttu-id="7aa21-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7aa21-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7aa21-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7aa21-128">Request body</span></span>
<span data-ttu-id="7aa21-129">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="7aa21-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="7aa21-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="7aa21-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="7aa21-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="7aa21-131">Property</span></span>|<span data-ttu-id="7aa21-132">Тип</span><span class="sxs-lookup"><span data-stu-id="7aa21-132">Type</span></span>|<span data-ttu-id="7aa21-133">Описание</span><span class="sxs-lookup"><span data-stu-id="7aa21-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7aa21-134">resource</span><span class="sxs-lookup"><span data-stu-id="7aa21-134">resource</span></span>|<span data-ttu-id="7aa21-135">String</span><span class="sxs-lookup"><span data-stu-id="7aa21-135">String</span></span>|<span data-ttu-id="7aa21-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="7aa21-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7aa21-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="7aa21-137">Response</span></span>
<span data-ttu-id="7aa21-138">Если успешно завершена, эта функция возвращает `200 OK` код ответа и семейства [roleScopeTag](../resources/intune-rbac-rolescopetag.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7aa21-138">If successful, this function returns a `200 OK` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7aa21-139">Пример</span><span class="sxs-lookup"><span data-stu-id="7aa21-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="7aa21-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="7aa21-140">Request</span></span>
<span data-ttu-id="7aa21-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7aa21-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getRoleScopeTagsByResource(resource='parameterValue')
```

### <a name="response"></a><span data-ttu-id="7aa21-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="7aa21-142">Response</span></span>
<span data-ttu-id="7aa21-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7aa21-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



