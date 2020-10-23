---
title: Удаление Виндовсоффицеклиентконфигуратион
description: Удаление определенной политики, не относящейся к безопасности.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c9ab26b542e9618966066aed659b2133d0431793
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48714901"
---
# <a name="delete-windowsofficeclientconfiguration"></a><span data-ttu-id="09bbe-103">Удаление Виндовсоффицеклиентконфигуратион</span><span class="sxs-lookup"><span data-stu-id="09bbe-103">Delete windowsOfficeClientConfiguration</span></span>

<span data-ttu-id="09bbe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09bbe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="09bbe-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09bbe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09bbe-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="09bbe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09bbe-107">Удаление определенной политики, не относящейся к безопасности.</span><span class="sxs-lookup"><span data-stu-id="09bbe-107">Delete a specific non-security policy.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="09bbe-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="09bbe-108">Prerequisites</span></span>
<span data-ttu-id="09bbe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09bbe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09bbe-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="09bbe-111">Permission type</span></span>|<span data-ttu-id="09bbe-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="09bbe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09bbe-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="09bbe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="09bbe-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09bbe-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="09bbe-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="09bbe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09bbe-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09bbe-116">Not supported.</span></span>|
|<span data-ttu-id="09bbe-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="09bbe-117">Application</span></span>|<span data-ttu-id="09bbe-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09bbe-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="09bbe-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="09bbe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /officeConfiguration/clientConfigurations/{key}
```

## <a name="request-headers"></a><span data-ttu-id="09bbe-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="09bbe-120">Request headers</span></span>
|<span data-ttu-id="09bbe-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="09bbe-121">Header</span></span>|<span data-ttu-id="09bbe-122">Значение</span><span class="sxs-lookup"><span data-stu-id="09bbe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09bbe-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="09bbe-123">Authorization</span></span>|<span data-ttu-id="09bbe-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="09bbe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09bbe-125">Accept</span><span class="sxs-lookup"><span data-stu-id="09bbe-125">Accept</span></span>|<span data-ttu-id="09bbe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="09bbe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09bbe-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="09bbe-127">Request body</span></span>
<span data-ttu-id="09bbe-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="09bbe-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09bbe-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="09bbe-129">Response</span></span>
<span data-ttu-id="09bbe-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="09bbe-130">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="09bbe-131">Пример</span><span class="sxs-lookup"><span data-stu-id="09bbe-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="09bbe-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="09bbe-132">Request</span></span>
<span data-ttu-id="09bbe-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="09bbe-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}
```

### <a name="response"></a><span data-ttu-id="09bbe-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="09bbe-134">Response</span></span>
<span data-ttu-id="09bbe-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="09bbe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
```





