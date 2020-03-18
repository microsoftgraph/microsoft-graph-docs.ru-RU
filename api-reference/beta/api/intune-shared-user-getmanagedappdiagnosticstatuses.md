---
title: Функция getManagedAppDiagnosticStatuses
description: Получает состояние диагностической проверки для определенного пользователя.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1cd9d5ccf9477b0db5aec803fbe1b18482f49c32
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800559"
---
# <a name="getmanagedappdiagnosticstatuses-function"></a><span data-ttu-id="da3e7-103">Функция getManagedAppDiagnosticStatuses</span><span class="sxs-lookup"><span data-stu-id="da3e7-103">getManagedAppDiagnosticStatuses function</span></span>

> <span data-ttu-id="da3e7-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="da3e7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="da3e7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da3e7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="da3e7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="da3e7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da3e7-107">Получает состояние диагностической проверки для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="da3e7-107">Gets diagnostics validation status for a given user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="da3e7-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="da3e7-108">Prerequisites</span></span>
<span data-ttu-id="da3e7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da3e7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da3e7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="da3e7-111">Permission type</span></span>|<span data-ttu-id="da3e7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="da3e7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da3e7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="da3e7-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="da3e7-114">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="da3e7-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="da3e7-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="da3e7-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="da3e7-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="da3e7-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da3e7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da3e7-117">Not supported.</span></span>|
|<span data-ttu-id="da3e7-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="da3e7-118">Application</span></span>||
| <span data-ttu-id="da3e7-119">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="da3e7-119">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="da3e7-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="da3e7-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="da3e7-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="da3e7-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppDiagnosticStatuses
```

## <a name="request-headers"></a><span data-ttu-id="da3e7-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="da3e7-122">Request headers</span></span>
|<span data-ttu-id="da3e7-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="da3e7-123">Header</span></span>|<span data-ttu-id="da3e7-124">Значение</span><span class="sxs-lookup"><span data-stu-id="da3e7-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da3e7-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="da3e7-125">Authorization</span></span>|<span data-ttu-id="da3e7-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="da3e7-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da3e7-127">Accept</span><span class="sxs-lookup"><span data-stu-id="da3e7-127">Accept</span></span>|<span data-ttu-id="da3e7-128">application/json</span><span class="sxs-lookup"><span data-stu-id="da3e7-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da3e7-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="da3e7-129">Request body</span></span>
<span data-ttu-id="da3e7-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="da3e7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da3e7-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="da3e7-131">Response</span></span>
<span data-ttu-id="da3e7-132">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="da3e7-132">If successful, this function returns a `200 OK` response code and a [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da3e7-133">Пример</span><span class="sxs-lookup"><span data-stu-id="da3e7-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="da3e7-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="da3e7-134">Request</span></span>
<span data-ttu-id="da3e7-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="da3e7-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedAppDiagnosticStatuses
```

### <a name="response"></a><span data-ttu-id="da3e7-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="da3e7-136">Response</span></span>
<span data-ttu-id="da3e7-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="da3e7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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













