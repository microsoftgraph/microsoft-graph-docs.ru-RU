---
title: Функция Жетролескопетагсбидс
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 40b228a59a426d09d760edb1490b890d91c69940
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538191"
---
# <a name="getrolescopetagsbyids-function"></a><span data-ttu-id="f0e30-103">Функция Жетролескопетагсбидс</span><span class="sxs-lookup"><span data-stu-id="f0e30-103">getRoleScopeTagsByIds function</span></span>

> <span data-ttu-id="f0e30-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f0e30-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f0e30-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0e30-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f0e30-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f0e30-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0e30-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="f0e30-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f0e30-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f0e30-108">Prerequisites</span></span>
<span data-ttu-id="f0e30-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0e30-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0e30-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f0e30-111">Permission type</span></span>|<span data-ttu-id="f0e30-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f0e30-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0e30-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f0e30-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f0e30-114">&nbsp; &nbsp; **Управление доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="f0e30-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="f0e30-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0e30-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="f0e30-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f0e30-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0e30-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0e30-117">Not supported.</span></span>|
|<span data-ttu-id="f0e30-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="f0e30-118">Application</span></span>||
| <span data-ttu-id="f0e30-119">&nbsp; &nbsp; **Управление доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="f0e30-119">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="f0e30-120">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0e30-120">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0e30-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f0e30-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getRoleScopeTagsByIds
```

## <a name="request-headers"></a><span data-ttu-id="f0e30-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f0e30-122">Request headers</span></span>
|<span data-ttu-id="f0e30-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f0e30-123">Header</span></span>|<span data-ttu-id="f0e30-124">Значение</span><span class="sxs-lookup"><span data-stu-id="f0e30-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0e30-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f0e30-125">Authorization</span></span>|<span data-ttu-id="f0e30-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f0e30-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0e30-127">Accept</span><span class="sxs-lookup"><span data-stu-id="f0e30-127">Accept</span></span>|<span data-ttu-id="f0e30-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f0e30-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0e30-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f0e30-129">Request body</span></span>
<span data-ttu-id="f0e30-130">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="f0e30-130">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="f0e30-131">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="f0e30-131">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="f0e30-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="f0e30-132">Property</span></span>|<span data-ttu-id="f0e30-133">Тип</span><span class="sxs-lookup"><span data-stu-id="f0e30-133">Type</span></span>|<span data-ttu-id="f0e30-134">Описание</span><span class="sxs-lookup"><span data-stu-id="f0e30-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0e30-135">ids</span><span class="sxs-lookup"><span data-stu-id="f0e30-135">ids</span></span>|<span data-ttu-id="f0e30-136">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f0e30-136">String collection</span></span>|<span data-ttu-id="f0e30-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f0e30-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f0e30-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="f0e30-138">Response</span></span>
<span data-ttu-id="f0e30-139">В случае успеха эта функция возвращает код `200 OK` отклика и коллекцию [ролескопетаг](../resources/intune-rbac-rolescopetag.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f0e30-139">If successful, this function returns a `200 OK` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0e30-140">Пример</span><span class="sxs-lookup"><span data-stu-id="f0e30-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="f0e30-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="f0e30-141">Request</span></span>
<span data-ttu-id="f0e30-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f0e30-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getRoleScopeTagsByIds(ids=[
  "Ids value"
])
```

### <a name="response"></a><span data-ttu-id="f0e30-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0e30-143">Response</span></span>
<span data-ttu-id="f0e30-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f0e30-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









