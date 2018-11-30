---
title: функция getRoleScopeTagsByResource
description: Н/Д
ms.openlocfilehash: 10c440464224877865e74d9c9fe1750088241af7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081089"
---
# <a name="getrolescopetagsbyresource-function"></a><span data-ttu-id="ba839-103">функция getRoleScopeTagsByResource</span><span class="sxs-lookup"><span data-stu-id="ba839-103">getRoleScopeTagsByResource function</span></span>

> <span data-ttu-id="ba839-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ba839-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ba839-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba839-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ba839-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ba839-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ba839-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ba839-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ba839-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ba839-108">Prerequisites</span></span>
<span data-ttu-id="ba839-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba839-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba839-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba839-111">Permission type</span></span>|<span data-ttu-id="ba839-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba839-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba839-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba839-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ba839-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="ba839-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="ba839-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba839-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba839-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba839-116">Not supported.</span></span>|
|<span data-ttu-id="ba839-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ba839-117">Application</span></span>|<span data-ttu-id="ba839-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba839-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba839-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba839-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getRoleScopeTagsByResource
```

## <a name="request-headers"></a><span data-ttu-id="ba839-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ba839-120">Request headers</span></span>
|<span data-ttu-id="ba839-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ba839-121">Header</span></span>|<span data-ttu-id="ba839-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ba839-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba839-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba839-123">Authorization</span></span>|<span data-ttu-id="ba839-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ba839-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba839-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ba839-125">Accept</span></span>|<span data-ttu-id="ba839-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ba839-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba839-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ba839-127">Request body</span></span>
<span data-ttu-id="ba839-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="ba839-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="ba839-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="ba839-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="ba839-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ba839-130">Property</span></span>|<span data-ttu-id="ba839-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ba839-131">Type</span></span>|<span data-ttu-id="ba839-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ba839-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba839-133">resource</span><span class="sxs-lookup"><span data-stu-id="ba839-133">resource</span></span>|<span data-ttu-id="ba839-134">String</span><span class="sxs-lookup"><span data-stu-id="ba839-134">String</span></span>|<span data-ttu-id="ba839-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ba839-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ba839-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="ba839-136">Response</span></span>
<span data-ttu-id="ba839-137">Если успешно завершена, эта функция возвращает `200 OK` код ответа и семейства [roleScopeTag](../resources/intune-rbac-rolescopetag.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ba839-137">If successful, this function returns a `200 OK` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba839-138">Пример</span><span class="sxs-lookup"><span data-stu-id="ba839-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="ba839-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba839-139">Request</span></span>
<span data-ttu-id="ba839-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ba839-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getRoleScopeTagsByResource(resource='parameterValue')
```

### <a name="response"></a><span data-ttu-id="ba839-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="ba839-141">Response</span></span>
<span data-ttu-id="ba839-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="ba839-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





