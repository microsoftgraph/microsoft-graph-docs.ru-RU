---
title: Функция getManagedAppDiagnosticStatuses
description: Получает состояние диагностической проверки для определенного пользователя.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ce1611c0e672b19d01c56809b59a1970293fd532
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35726166"
---
# <a name="getmanagedappdiagnosticstatuses-function"></a><span data-ttu-id="39968-103">Функция getManagedAppDiagnosticStatuses</span><span class="sxs-lookup"><span data-stu-id="39968-103">getManagedAppDiagnosticStatuses function</span></span>

> <span data-ttu-id="39968-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39968-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="39968-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="39968-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39968-106">Получает состояние диагностической проверки для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="39968-106">Gets diagnostics validation status for a given user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="39968-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="39968-107">Prerequisites</span></span>
<span data-ttu-id="39968-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39968-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39968-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="39968-110">Permission type</span></span>|<span data-ttu-id="39968-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="39968-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="39968-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="39968-112">Delegated (work or school account)</span></span>|<span data-ttu-id="39968-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="39968-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="39968-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="39968-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39968-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39968-115">Not supported.</span></span>|
|<span data-ttu-id="39968-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="39968-116">Application</span></span>|<span data-ttu-id="39968-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39968-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="39968-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="39968-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppDiagnosticStatuses
```

## <a name="request-headers"></a><span data-ttu-id="39968-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="39968-119">Request headers</span></span>
|<span data-ttu-id="39968-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="39968-120">Header</span></span>|<span data-ttu-id="39968-121">Значение</span><span class="sxs-lookup"><span data-stu-id="39968-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="39968-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="39968-122">Authorization</span></span>|<span data-ttu-id="39968-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="39968-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="39968-124">Accept</span><span class="sxs-lookup"><span data-stu-id="39968-124">Accept</span></span>|<span data-ttu-id="39968-125">application/json</span><span class="sxs-lookup"><span data-stu-id="39968-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="39968-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="39968-126">Request body</span></span>
<span data-ttu-id="39968-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="39968-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="39968-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="39968-128">Response</span></span>
<span data-ttu-id="39968-129">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="39968-129">If successful, this function returns a `200 OK` response code and a [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39968-130">Пример</span><span class="sxs-lookup"><span data-stu-id="39968-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="39968-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="39968-131">Request</span></span>
<span data-ttu-id="39968-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="39968-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedAppDiagnosticStatuses
```

### <a name="response"></a><span data-ttu-id="39968-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="39968-133">Response</span></span>
<span data-ttu-id="39968-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="39968-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





