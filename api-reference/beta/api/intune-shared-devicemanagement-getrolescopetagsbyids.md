---
title: Функция Жетролескопетагсбидс
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6e234f938d7c534bc699f1c7004fd3cf01f479ce
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37194643"
---
# <a name="getrolescopetagsbyids-function"></a><span data-ttu-id="ff7aa-103">Функция Жетролескопетагсбидс</span><span class="sxs-lookup"><span data-stu-id="ff7aa-103">getRoleScopeTagsByIds function</span></span>

> <span data-ttu-id="ff7aa-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ff7aa-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ff7aa-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff7aa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ff7aa-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ff7aa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff7aa-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ff7aa-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ff7aa-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ff7aa-108">Prerequisites</span></span>
<span data-ttu-id="ff7aa-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff7aa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff7aa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ff7aa-111">Permission type</span></span>|<span data-ttu-id="ff7aa-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ff7aa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff7aa-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ff7aa-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ff7aa-114">&nbsp; &nbsp; **Управление доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="ff7aa-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="ff7aa-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="ff7aa-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="ff7aa-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ff7aa-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff7aa-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff7aa-117">Not supported.</span></span>|
|<span data-ttu-id="ff7aa-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ff7aa-118">Application</span></span>||
| <span data-ttu-id="ff7aa-119">&nbsp; &nbsp; **Управление доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="ff7aa-119">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="ff7aa-120">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="ff7aa-120">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff7aa-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ff7aa-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getRoleScopeTagsByIds
```

## <a name="request-headers"></a><span data-ttu-id="ff7aa-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ff7aa-122">Request headers</span></span>
|<span data-ttu-id="ff7aa-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ff7aa-123">Header</span></span>|<span data-ttu-id="ff7aa-124">Значение</span><span class="sxs-lookup"><span data-stu-id="ff7aa-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff7aa-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ff7aa-125">Authorization</span></span>|<span data-ttu-id="ff7aa-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ff7aa-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff7aa-127">Accept</span><span class="sxs-lookup"><span data-stu-id="ff7aa-127">Accept</span></span>|<span data-ttu-id="ff7aa-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ff7aa-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff7aa-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ff7aa-129">Request body</span></span>
<span data-ttu-id="ff7aa-130">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="ff7aa-130">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="ff7aa-131">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="ff7aa-131">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="ff7aa-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff7aa-132">Property</span></span>|<span data-ttu-id="ff7aa-133">Тип</span><span class="sxs-lookup"><span data-stu-id="ff7aa-133">Type</span></span>|<span data-ttu-id="ff7aa-134">Описание</span><span class="sxs-lookup"><span data-stu-id="ff7aa-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff7aa-135">ids</span><span class="sxs-lookup"><span data-stu-id="ff7aa-135">ids</span></span>|<span data-ttu-id="ff7aa-136">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ff7aa-136">String collection</span></span>|<span data-ttu-id="ff7aa-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ff7aa-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ff7aa-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="ff7aa-138">Response</span></span>
<span data-ttu-id="ff7aa-139">В случае успеха эта функция возвращает код `200 OK` отклика и коллекцию [ролескопетаг](../resources/intune-rbac-rolescopetag.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ff7aa-139">If successful, this function returns a `200 OK` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff7aa-140">Пример</span><span class="sxs-lookup"><span data-stu-id="ff7aa-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="ff7aa-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="ff7aa-141">Request</span></span>
<span data-ttu-id="ff7aa-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ff7aa-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getRoleScopeTagsByIds(ids=[
  "Ids value"
])
```

### <a name="response"></a><span data-ttu-id="ff7aa-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff7aa-143">Response</span></span>
<span data-ttu-id="ff7aa-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ff7aa-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







