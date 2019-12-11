---
title: Удаление Девицеконфигуратионконфликтсуммари
description: Удаляет объект Девицеконфигуратионконфликтсуммари.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8de16ca70dc9674cde8407641586c460d989874b
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39949450"
---
# <a name="delete-deviceconfigurationconflictsummary"></a><span data-ttu-id="d7bce-103">Удаление Девицеконфигуратионконфликтсуммари</span><span class="sxs-lookup"><span data-stu-id="d7bce-103">Delete deviceConfigurationConflictSummary</span></span>

> <span data-ttu-id="d7bce-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7bce-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7bce-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d7bce-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7bce-106">Удаляет объект [девицеконфигуратионконфликтсуммари](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).</span><span class="sxs-lookup"><span data-stu-id="d7bce-106">Deletes a [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d7bce-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d7bce-107">Prerequisites</span></span>
<span data-ttu-id="d7bce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7bce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7bce-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d7bce-110">Permission type</span></span>|<span data-ttu-id="d7bce-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d7bce-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7bce-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d7bce-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d7bce-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7bce-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d7bce-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d7bce-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7bce-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7bce-115">Not supported.</span></span>|
|<span data-ttu-id="d7bce-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d7bce-116">Application</span></span>|<span data-ttu-id="d7bce-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7bce-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7bce-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7bce-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="d7bce-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d7bce-119">Request headers</span></span>
|<span data-ttu-id="d7bce-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d7bce-120">Header</span></span>|<span data-ttu-id="d7bce-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d7bce-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7bce-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d7bce-122">Authorization</span></span>|<span data-ttu-id="d7bce-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d7bce-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7bce-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d7bce-124">Accept</span></span>|<span data-ttu-id="d7bce-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d7bce-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7bce-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d7bce-126">Request body</span></span>
<span data-ttu-id="d7bce-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d7bce-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7bce-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="d7bce-128">Response</span></span>
<span data-ttu-id="d7bce-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d7bce-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d7bce-130">Пример</span><span class="sxs-lookup"><span data-stu-id="d7bce-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d7bce-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7bce-131">Request</span></span>
<span data-ttu-id="d7bce-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d7bce-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
```

### <a name="response"></a><span data-ttu-id="d7bce-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="d7bce-133">Response</span></span>
<span data-ttu-id="d7bce-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d7bce-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





