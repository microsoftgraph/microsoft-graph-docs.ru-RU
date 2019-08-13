---
title: Функция getManagedAppDiagnosticStatuses
description: Получает состояние диагностической проверки для определенного пользователя.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4a21faa0be644e9b44e456c7ffa7c3d93829795a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350650"
---
# <a name="getmanagedappdiagnosticstatuses-function"></a><span data-ttu-id="365da-103">Функция getManagedAppDiagnosticStatuses</span><span class="sxs-lookup"><span data-stu-id="365da-103">getManagedAppDiagnosticStatuses function</span></span>

> <span data-ttu-id="365da-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="365da-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="365da-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="365da-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="365da-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="365da-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="365da-107">Получает состояние диагностической проверки для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="365da-107">Gets diagnostics validation status for a given user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="365da-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="365da-108">Prerequisites</span></span>
<span data-ttu-id="365da-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="365da-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="365da-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="365da-111">Permission type</span></span>|<span data-ttu-id="365da-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="365da-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="365da-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="365da-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="365da-114">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="365da-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="365da-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="365da-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="365da-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="365da-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="365da-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="365da-117">Not supported.</span></span>|
|<span data-ttu-id="365da-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="365da-118">Application</span></span>|<span data-ttu-id="365da-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="365da-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="365da-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="365da-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppDiagnosticStatuses
```

## <a name="request-headers"></a><span data-ttu-id="365da-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="365da-121">Request headers</span></span>
|<span data-ttu-id="365da-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="365da-122">Header</span></span>|<span data-ttu-id="365da-123">Значение</span><span class="sxs-lookup"><span data-stu-id="365da-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="365da-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="365da-124">Authorization</span></span>|<span data-ttu-id="365da-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="365da-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="365da-126">Accept</span><span class="sxs-lookup"><span data-stu-id="365da-126">Accept</span></span>|<span data-ttu-id="365da-127">application/json</span><span class="sxs-lookup"><span data-stu-id="365da-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="365da-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="365da-128">Request body</span></span>
<span data-ttu-id="365da-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="365da-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="365da-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="365da-130">Response</span></span>
<span data-ttu-id="365da-131">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="365da-131">If successful, this function returns a `200 OK` response code and a [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="365da-132">Пример</span><span class="sxs-lookup"><span data-stu-id="365da-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="365da-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="365da-133">Request</span></span>
<span data-ttu-id="365da-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="365da-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedAppDiagnosticStatuses
```

### <a name="response"></a><span data-ttu-id="365da-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="365da-135">Response</span></span>
<span data-ttu-id="365da-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="365da-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 249

{
  "value": [
    {
      "@odata.type": "microsoft.graph.managedAppDiagnosticStatus",
      "validationName": "Validation Name value",
      "state": "State value",
      "mitigationInstruction": "Mitigation Instruction value"
    }
  ]
}
```









