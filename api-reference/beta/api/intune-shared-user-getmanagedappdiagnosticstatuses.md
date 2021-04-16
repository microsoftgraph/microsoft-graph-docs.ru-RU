---
title: Функция getManagedAppDiagnosticStatuses
description: Получает состояние диагностической проверки для определенного пользователя.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: faea09447153988b7ca8ecf86b013fea83a50920
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51865105"
---
# <a name="getmanagedappdiagnosticstatuses-function"></a><span data-ttu-id="8dd82-103">Функция getManagedAppDiagnosticStatuses</span><span class="sxs-lookup"><span data-stu-id="8dd82-103">getManagedAppDiagnosticStatuses function</span></span>

<span data-ttu-id="8dd82-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8dd82-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8dd82-105">**Важно:** API в версии /бета-версии в Microsoft Graph могут изменяться.</span><span class="sxs-lookup"><span data-stu-id="8dd82-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8dd82-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8dd82-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8dd82-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8dd82-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8dd82-108">Получает состояние диагностической проверки для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="8dd82-108">Gets diagnostics validation status for a given user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8dd82-109">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8dd82-109">Prerequisites</span></span>
<span data-ttu-id="8dd82-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8dd82-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8dd82-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8dd82-112">Permission type</span></span>|<span data-ttu-id="8dd82-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8dd82-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8dd82-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8dd82-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8dd82-115">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="8dd82-115">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="8dd82-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8dd82-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="8dd82-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8dd82-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8dd82-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8dd82-118">Not supported.</span></span>|
|<span data-ttu-id="8dd82-119">Для приложения</span><span class="sxs-lookup"><span data-stu-id="8dd82-119">Application</span></span>||
| <span data-ttu-id="8dd82-120">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="8dd82-120">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="8dd82-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8dd82-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8dd82-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8dd82-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppDiagnosticStatuses
```

## <a name="request-headers"></a><span data-ttu-id="8dd82-123">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8dd82-123">Request headers</span></span>
|<span data-ttu-id="8dd82-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8dd82-124">Header</span></span>|<span data-ttu-id="8dd82-125">Значение</span><span class="sxs-lookup"><span data-stu-id="8dd82-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8dd82-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8dd82-126">Authorization</span></span>|<span data-ttu-id="8dd82-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8dd82-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8dd82-128">Accept</span><span class="sxs-lookup"><span data-stu-id="8dd82-128">Accept</span></span>|<span data-ttu-id="8dd82-129">application/json</span><span class="sxs-lookup"><span data-stu-id="8dd82-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8dd82-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8dd82-130">Request body</span></span>
<span data-ttu-id="8dd82-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8dd82-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8dd82-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="8dd82-132">Response</span></span>
<span data-ttu-id="8dd82-133">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8dd82-133">If successful, this function returns a `200 OK` response code and a [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8dd82-134">Пример</span><span class="sxs-lookup"><span data-stu-id="8dd82-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="8dd82-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="8dd82-135">Request</span></span>
<span data-ttu-id="8dd82-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8dd82-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedAppDiagnosticStatuses
```

### <a name="response"></a><span data-ttu-id="8dd82-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="8dd82-137">Response</span></span>
<span data-ttu-id="8dd82-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8dd82-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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













