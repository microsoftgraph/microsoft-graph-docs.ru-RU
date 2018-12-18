---
title: функция getRoleScopeTagsByIds
description: Н/Д
author: tfitzmac
ms.openlocfilehash: b6708a605ad0c528e691b0a9a3a218e178ff7730
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342492"
---
# <a name="getrolescopetagsbyids-function"></a><span data-ttu-id="6fefc-103">функция getRoleScopeTagsByIds</span><span class="sxs-lookup"><span data-stu-id="6fefc-103">getRoleScopeTagsByIds function</span></span>

> <span data-ttu-id="6fefc-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6fefc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6fefc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6fefc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6fefc-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6fefc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6fefc-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="6fefc-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6fefc-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="6fefc-108">Prerequisites</span></span>
<span data-ttu-id="6fefc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6fefc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6fefc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6fefc-111">Permission type</span></span>|<span data-ttu-id="6fefc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6fefc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6fefc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6fefc-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="6fefc-114">&nbsp;&nbsp; **Управления доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="6fefc-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="6fefc-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="6fefc-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="6fefc-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6fefc-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6fefc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6fefc-117">Not supported.</span></span>|
|<span data-ttu-id="6fefc-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6fefc-118">Application</span></span>|<span data-ttu-id="6fefc-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6fefc-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6fefc-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6fefc-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getRoleScopeTagsByIds
```

## <a name="request-headers"></a><span data-ttu-id="6fefc-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6fefc-121">Request headers</span></span>
|<span data-ttu-id="6fefc-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6fefc-122">Header</span></span>|<span data-ttu-id="6fefc-123">Значение</span><span class="sxs-lookup"><span data-stu-id="6fefc-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6fefc-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6fefc-124">Authorization</span></span>|<span data-ttu-id="6fefc-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6fefc-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6fefc-126">Accept</span><span class="sxs-lookup"><span data-stu-id="6fefc-126">Accept</span></span>|<span data-ttu-id="6fefc-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6fefc-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6fefc-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6fefc-128">Request body</span></span>
<span data-ttu-id="6fefc-129">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="6fefc-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="6fefc-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="6fefc-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="6fefc-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="6fefc-131">Property</span></span>|<span data-ttu-id="6fefc-132">Тип</span><span class="sxs-lookup"><span data-stu-id="6fefc-132">Type</span></span>|<span data-ttu-id="6fefc-133">Описание</span><span class="sxs-lookup"><span data-stu-id="6fefc-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fefc-134">ids</span><span class="sxs-lookup"><span data-stu-id="6fefc-134">ids</span></span>|<span data-ttu-id="6fefc-135">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="6fefc-135">String collection</span></span>|<span data-ttu-id="6fefc-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="6fefc-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6fefc-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="6fefc-137">Response</span></span>
<span data-ttu-id="6fefc-138">Если успешно завершена, эта функция возвращает `200 OK` код ответа и семейства [roleScopeTag](../resources/intune-rbac-rolescopetag.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6fefc-138">If successful, this function returns a `200 OK` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6fefc-139">Пример</span><span class="sxs-lookup"><span data-stu-id="6fefc-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="6fefc-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="6fefc-140">Request</span></span>
<span data-ttu-id="6fefc-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6fefc-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getRoleScopeTagsByIds(ids=[
  "Ids value"
])
```

### <a name="response"></a><span data-ttu-id="6fefc-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="6fefc-142">Response</span></span>
<span data-ttu-id="6fefc-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6fefc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



