---
title: функция getRoleScopeTagsByIds
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4eeb89d0b3636ad20f9b59ad1ee9db867e5481e8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929706"
---
# <a name="getrolescopetagsbyids-function"></a><span data-ttu-id="0523e-103">функция getRoleScopeTagsByIds</span><span class="sxs-lookup"><span data-stu-id="0523e-103">getRoleScopeTagsByIds function</span></span>

> <span data-ttu-id="0523e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0523e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0523e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0523e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0523e-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0523e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0523e-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="0523e-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0523e-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="0523e-108">Prerequisites</span></span>
<span data-ttu-id="0523e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0523e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0523e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0523e-111">Permission type</span></span>|<span data-ttu-id="0523e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0523e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0523e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0523e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0523e-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="0523e-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="0523e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0523e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0523e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0523e-116">Not supported.</span></span>|
|<span data-ttu-id="0523e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0523e-117">Application</span></span>|<span data-ttu-id="0523e-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0523e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0523e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0523e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getRoleScopeTagsByIds
```

## <a name="request-headers"></a><span data-ttu-id="0523e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0523e-120">Request headers</span></span>
|<span data-ttu-id="0523e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0523e-121">Header</span></span>|<span data-ttu-id="0523e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0523e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0523e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0523e-123">Authorization</span></span>|<span data-ttu-id="0523e-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0523e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0523e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0523e-125">Accept</span></span>|<span data-ttu-id="0523e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0523e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0523e-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0523e-127">Request body</span></span>
<span data-ttu-id="0523e-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="0523e-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="0523e-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="0523e-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="0523e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0523e-130">Property</span></span>|<span data-ttu-id="0523e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0523e-131">Type</span></span>|<span data-ttu-id="0523e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0523e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0523e-133">ids</span><span class="sxs-lookup"><span data-stu-id="0523e-133">ids</span></span>|<span data-ttu-id="0523e-134">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="0523e-134">String collection</span></span>|<span data-ttu-id="0523e-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="0523e-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0523e-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="0523e-136">Response</span></span>
<span data-ttu-id="0523e-137">Если успешно завершена, эта функция возвращает `200 OK` код ответа и семейства [roleScopeTag](../resources/intune-rbac-rolescopetag.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0523e-137">If successful, this function returns a `200 OK` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0523e-138">Пример</span><span class="sxs-lookup"><span data-stu-id="0523e-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="0523e-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="0523e-139">Request</span></span>
<span data-ttu-id="0523e-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0523e-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getRoleScopeTagsByIds(ids=[
  "Ids value"
])
```

### <a name="response"></a><span data-ttu-id="0523e-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="0523e-141">Response</span></span>
<span data-ttu-id="0523e-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0523e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





