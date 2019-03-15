---
title: Функция Жетролескопетагсбидс
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 556d83629a675c3c112105a1126176823af031c0
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571657"
---
# <a name="getrolescopetagsbyids-function"></a><span data-ttu-id="6f30a-103">Функция Жетролескопетагсбидс</span><span class="sxs-lookup"><span data-stu-id="6f30a-103">getRoleScopeTagsByIds function</span></span>

> <span data-ttu-id="6f30a-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6f30a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6f30a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f30a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6f30a-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6f30a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f30a-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="6f30a-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6f30a-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6f30a-108">Prerequisites</span></span>
<span data-ttu-id="6f30a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6f30a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6f30a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f30a-111">Permission type</span></span>|<span data-ttu-id="6f30a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f30a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f30a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f30a-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="6f30a-114">&nbsp;&nbsp; **Управление доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="6f30a-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="6f30a-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f30a-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="6f30a-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f30a-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f30a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f30a-117">Not supported.</span></span>|
|<span data-ttu-id="6f30a-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6f30a-118">Application</span></span>|<span data-ttu-id="6f30a-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f30a-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f30a-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f30a-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getRoleScopeTagsByIds
```

## <a name="request-headers"></a><span data-ttu-id="6f30a-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6f30a-121">Request headers</span></span>
|<span data-ttu-id="6f30a-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6f30a-122">Header</span></span>|<span data-ttu-id="6f30a-123">Значение</span><span class="sxs-lookup"><span data-stu-id="6f30a-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f30a-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6f30a-124">Authorization</span></span>|<span data-ttu-id="6f30a-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6f30a-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f30a-126">Accept</span><span class="sxs-lookup"><span data-stu-id="6f30a-126">Accept</span></span>|<span data-ttu-id="6f30a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6f30a-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f30a-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6f30a-128">Request body</span></span>
<span data-ttu-id="6f30a-129">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="6f30a-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="6f30a-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="6f30a-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="6f30a-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f30a-131">Property</span></span>|<span data-ttu-id="6f30a-132">Тип</span><span class="sxs-lookup"><span data-stu-id="6f30a-132">Type</span></span>|<span data-ttu-id="6f30a-133">Описание</span><span class="sxs-lookup"><span data-stu-id="6f30a-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f30a-134">ids</span><span class="sxs-lookup"><span data-stu-id="6f30a-134">ids</span></span>|<span data-ttu-id="6f30a-135">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6f30a-135">String collection</span></span>|<span data-ttu-id="6f30a-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="6f30a-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6f30a-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="6f30a-137">Response</span></span>
<span data-ttu-id="6f30a-138">В случае успеха эта функция возвращает код `200 OK` отклика и коллекцию [ролескопетаг](../resources/intune-rbac-rolescopetag.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6f30a-138">If successful, this function returns a `200 OK` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f30a-139">Пример</span><span class="sxs-lookup"><span data-stu-id="6f30a-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="6f30a-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f30a-140">Request</span></span>
<span data-ttu-id="6f30a-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f30a-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getRoleScopeTagsByIds(ids=[
  "Ids value"
])
```

### <a name="response"></a><span data-ttu-id="6f30a-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f30a-142">Response</span></span>
<span data-ttu-id="6f30a-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6f30a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



