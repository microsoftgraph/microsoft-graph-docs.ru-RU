---
title: Функция Жетассигнедролеидсфорлогжединусер
description: Извлекает назначенные определения ролей и назначения ролей для текущего пользователя, прошедшего проверку подлинности.
author: rolyon
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 61c42efdf0ae9b773f1bf136d2dccb011a687aad
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33898669"
---
# <a name="getassignedroleidsforloggedinuser-function"></a><span data-ttu-id="eb12c-103">Функция Жетассигнедролеидсфорлогжединусер</span><span class="sxs-lookup"><span data-stu-id="eb12c-103">getAssignedRoleIdsForLoggedInUser function</span></span>

> <span data-ttu-id="eb12c-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="eb12c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="eb12c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb12c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eb12c-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eb12c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb12c-107">Извлекает назначенные определения ролей и назначения ролей для текущего пользователя, прошедшего проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="eb12c-107">Retrieves the assigned role definitions and role assignments of the currently authenticated user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="eb12c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="eb12c-108">Prerequisites</span></span>
<span data-ttu-id="eb12c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb12c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb12c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eb12c-111">Permission type</span></span>|<span data-ttu-id="eb12c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="eb12c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb12c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eb12c-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="eb12c-114">&nbsp; &nbsp; **Управление доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="eb12c-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="eb12c-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="eb12c-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="eb12c-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eb12c-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb12c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb12c-117">Not supported.</span></span>|
|<span data-ttu-id="eb12c-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eb12c-118">Application</span></span>|<span data-ttu-id="eb12c-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb12c-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb12c-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eb12c-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getAssignedRoleIdsForLoggedInUser
```

## <a name="request-headers"></a><span data-ttu-id="eb12c-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eb12c-121">Request headers</span></span>
|<span data-ttu-id="eb12c-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eb12c-122">Header</span></span>|<span data-ttu-id="eb12c-123">Значение</span><span class="sxs-lookup"><span data-stu-id="eb12c-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb12c-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eb12c-124">Authorization</span></span>|<span data-ttu-id="eb12c-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eb12c-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb12c-126">Accept</span><span class="sxs-lookup"><span data-stu-id="eb12c-126">Accept</span></span>|<span data-ttu-id="eb12c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="eb12c-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb12c-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eb12c-128">Request body</span></span>
<span data-ttu-id="eb12c-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="eb12c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb12c-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="eb12c-130">Response</span></span>
<span data-ttu-id="eb12c-131">В случае успеха эта функция возвращает код `200 OK` отклика и объект **девицеандаппманажементассигнедролеид** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="eb12c-131">If successful, this function returns a `200 OK` response code and a **deviceAndAppManagementAssignedRoleId** in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb12c-132">Пример</span><span class="sxs-lookup"><span data-stu-id="eb12c-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="eb12c-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="eb12c-133">Request</span></span>
<span data-ttu-id="eb12c-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eb12c-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getAssignedRoleIdsForLoggedInUser
```

### <a name="response"></a><span data-ttu-id="eb12c-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb12c-135">Response</span></span>
<span data-ttu-id="eb12c-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="eb12c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 263

{
  "value": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignedRoleIds",
    "roleDefinitionIds": [
      "df52f163-f163-df52-63f1-52df63f152df"
    ],
    "roleAssignmentIds": [
      "1f35d53d-d53d-1f35-3dd5-351f3dd5351f"
    ]
  }
}
```





