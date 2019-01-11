---
title: Функция getEffectivePermissions
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 18c3774515cfd680e87b84828591313e67aab60a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885542"
---
# <a name="geteffectivepermissions-function"></a><span data-ttu-id="1879a-103">Функция getEffectivePermissions</span><span class="sxs-lookup"><span data-stu-id="1879a-103">getEffectivePermissions function</span></span>

> <span data-ttu-id="1879a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1879a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1879a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1879a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1879a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1879a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1879a-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1879a-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1879a-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="1879a-108">Prerequisites</span></span>
<span data-ttu-id="1879a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1879a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1879a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1879a-111">Permission type</span></span>|<span data-ttu-id="1879a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1879a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1879a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1879a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1879a-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="1879a-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="1879a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1879a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1879a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1879a-116">Not supported.</span></span>|
|<span data-ttu-id="1879a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1879a-117">Application</span></span>|<span data-ttu-id="1879a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1879a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1879a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1879a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="1879a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1879a-120">Request headers</span></span>
|<span data-ttu-id="1879a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1879a-121">Header</span></span>|<span data-ttu-id="1879a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1879a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1879a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1879a-123">Authorization</span></span>|<span data-ttu-id="1879a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1879a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1879a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1879a-125">Accept</span></span>|<span data-ttu-id="1879a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1879a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1879a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1879a-127">Request body</span></span>
<span data-ttu-id="1879a-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="1879a-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="1879a-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="1879a-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="1879a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1879a-130">Property</span></span>|<span data-ttu-id="1879a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1879a-131">Type</span></span>|<span data-ttu-id="1879a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1879a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1879a-133">scope</span><span class="sxs-lookup"><span data-stu-id="1879a-133">scope</span></span>|<span data-ttu-id="1879a-134">Строка</span><span class="sxs-lookup"><span data-stu-id="1879a-134">String</span></span>|<span data-ttu-id="1879a-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1879a-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="1879a-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="1879a-136">Response</span></span>
<span data-ttu-id="1879a-137">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию [rolePermission](../resources/intune-rbac-rolepermission.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1879a-137">If successful, this function returns a `200 OK` response code and a [rolePermission](../resources/intune-rbac-rolepermission.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1879a-138">Пример</span><span class="sxs-lookup"><span data-stu-id="1879a-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="1879a-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="1879a-139">Request</span></span>
<span data-ttu-id="1879a-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1879a-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getEffectivePermissions(scope='parameterValue')
```

### <a name="response"></a><span data-ttu-id="1879a-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="1879a-141">Response</span></span>
<span data-ttu-id="1879a-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1879a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 471

{
  "value": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "actions": [
        "Actions value"
      ],
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "notAllowedResourceActions": [
            "Not Allowed Resource Actions value"
          ]
        }
      ]
    }
  ]
}
```





