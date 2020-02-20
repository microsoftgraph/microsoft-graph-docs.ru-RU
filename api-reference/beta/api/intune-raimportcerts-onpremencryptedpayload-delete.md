---
title: Удаление Онпременкриптедпайлоад
description: Удаляет объект Онпременкриптедпайлоад.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 24a169a73363ceb125f281f96fb272edf81ee84d
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42161608"
---
# <a name="delete-onpremencryptedpayload"></a><span data-ttu-id="f5505-103">Удаление Онпременкриптедпайлоад</span><span class="sxs-lookup"><span data-stu-id="f5505-103">Delete onPremEncryptedPayload</span></span>

> <span data-ttu-id="f5505-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5505-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f5505-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f5505-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5505-106">Удаляет объект [онпременкриптедпайлоад](../resources/intune-raimportcerts-onpremencryptedpayload.md).</span><span class="sxs-lookup"><span data-stu-id="f5505-106">Deletes a [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f5505-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f5505-107">Prerequisites</span></span>
<span data-ttu-id="f5505-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5505-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5505-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f5505-110">Permission type</span></span>|<span data-ttu-id="f5505-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f5505-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5505-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f5505-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f5505-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5505-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f5505-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f5505-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5505-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5505-115">Not supported.</span></span>|
|<span data-ttu-id="f5505-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f5505-116">Application</span></span>|<span data-ttu-id="f5505-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5505-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5505-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f5505-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /onPremEncryptedPayloads/{onPremEncryptedPayloadsId}
```

## <a name="request-headers"></a><span data-ttu-id="f5505-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f5505-119">Request headers</span></span>
|<span data-ttu-id="f5505-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f5505-120">Header</span></span>|<span data-ttu-id="f5505-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f5505-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f5505-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5505-122">Authorization</span></span>|<span data-ttu-id="f5505-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f5505-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f5505-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f5505-124">Accept</span></span>|<span data-ttu-id="f5505-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f5505-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5505-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f5505-126">Request body</span></span>
<span data-ttu-id="f5505-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f5505-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5505-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5505-128">Response</span></span>
<span data-ttu-id="f5505-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f5505-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f5505-130">Пример</span><span class="sxs-lookup"><span data-stu-id="f5505-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f5505-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f5505-131">Request</span></span>
<span data-ttu-id="f5505-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f5505-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/onPremEncryptedPayloads/{onPremEncryptedPayloadsId}
```

### <a name="response"></a><span data-ttu-id="f5505-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5505-133">Response</span></span>
<span data-ttu-id="f5505-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f5505-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





