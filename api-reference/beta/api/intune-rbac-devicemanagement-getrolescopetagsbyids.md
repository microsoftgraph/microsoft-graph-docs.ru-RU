---
title: функция getRoleScopeTagsByIds
description: Н/Д
author: tfitzmac
ms.openlocfilehash: 6b2efeff02b7404aefce1e6acbfbc3a0aca663f8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351802"
---
# <a name="getrolescopetagsbyids-function"></a><span data-ttu-id="2b970-103">функция getRoleScopeTagsByIds</span><span class="sxs-lookup"><span data-stu-id="2b970-103">getRoleScopeTagsByIds function</span></span>

> <span data-ttu-id="2b970-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2b970-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2b970-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b970-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2b970-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2b970-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2b970-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2b970-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2b970-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="2b970-108">Prerequisites</span></span>
<span data-ttu-id="2b970-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b970-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b970-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b970-111">Permission type</span></span>|<span data-ttu-id="2b970-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b970-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b970-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b970-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2b970-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b970-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="2b970-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b970-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b970-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b970-116">Not supported.</span></span>|
|<span data-ttu-id="2b970-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2b970-117">Application</span></span>|<span data-ttu-id="2b970-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b970-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b970-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b970-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getRoleScopeTagsByIds
```

## <a name="request-headers"></a><span data-ttu-id="2b970-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2b970-120">Request headers</span></span>
|<span data-ttu-id="2b970-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2b970-121">Header</span></span>|<span data-ttu-id="2b970-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2b970-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b970-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2b970-123">Authorization</span></span>|<span data-ttu-id="2b970-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2b970-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b970-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2b970-125">Accept</span></span>|<span data-ttu-id="2b970-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2b970-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b970-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2b970-127">Request body</span></span>
<span data-ttu-id="2b970-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="2b970-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="2b970-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="2b970-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="2b970-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2b970-130">Property</span></span>|<span data-ttu-id="2b970-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2b970-131">Type</span></span>|<span data-ttu-id="2b970-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2b970-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b970-133">ids</span><span class="sxs-lookup"><span data-stu-id="2b970-133">ids</span></span>|<span data-ttu-id="2b970-134">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="2b970-134">String collection</span></span>|<span data-ttu-id="2b970-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2b970-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2b970-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="2b970-136">Response</span></span>
<span data-ttu-id="2b970-137">Если успешно завершена, эта функция возвращает `200 OK` код ответа и семейства [roleScopeTag](../resources/intune-rbac-rolescopetag.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2b970-137">If successful, this function returns a `200 OK` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b970-138">Пример</span><span class="sxs-lookup"><span data-stu-id="2b970-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="2b970-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b970-139">Request</span></span>
<span data-ttu-id="2b970-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b970-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getRoleScopeTagsByIds(ids=[
  "Ids value"
])
```

### <a name="response"></a><span data-ttu-id="2b970-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="2b970-141">Response</span></span>
<span data-ttu-id="2b970-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2b970-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





