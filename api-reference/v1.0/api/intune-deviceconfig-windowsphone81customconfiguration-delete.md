---
title: Удаление объекта windowsPhone81CustomConfiguration
description: Удаляет объект windowsPhone81CustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e6d2f2a15b71b7b7c22b63b8083fbf93886e2d7e
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250812"
---
# <a name="delete-windowsphone81customconfiguration"></a><span data-ttu-id="3a152-103">Удаление объекта windowsPhone81CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="3a152-103">Delete windowsPhone81CustomConfiguration</span></span>

> <span data-ttu-id="3a152-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3a152-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a152-105">Удаляет объект [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3a152-105">Deletes a [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3a152-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3a152-106">Prerequisites</span></span>
<span data-ttu-id="3a152-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3a152-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3a152-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a152-109">Permission type</span></span>|<span data-ttu-id="3a152-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a152-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a152-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a152-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3a152-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a152-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3a152-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a152-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a152-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a152-114">Not supported.</span></span>|
|<span data-ttu-id="3a152-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3a152-115">Application</span></span>|<span data-ttu-id="3a152-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a152-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a152-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a152-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="3a152-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3a152-118">Request headers</span></span>
|<span data-ttu-id="3a152-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3a152-119">Header</span></span>|<span data-ttu-id="3a152-120">Значение</span><span class="sxs-lookup"><span data-stu-id="3a152-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a152-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a152-121">Authorization</span></span>|<span data-ttu-id="3a152-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3a152-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a152-123">Accept</span><span class="sxs-lookup"><span data-stu-id="3a152-123">Accept</span></span>|<span data-ttu-id="3a152-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3a152-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a152-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3a152-125">Request body</span></span>
<span data-ttu-id="3a152-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3a152-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a152-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a152-127">Response</span></span>
<span data-ttu-id="3a152-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3a152-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3a152-129">Пример</span><span class="sxs-lookup"><span data-stu-id="3a152-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="3a152-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a152-130">Request</span></span>
<span data-ttu-id="3a152-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3a152-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="3a152-132">Отклик
</span><span class="sxs-lookup"><span data-stu-id="3a152-132">Response</span></span>
<span data-ttu-id="3a152-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3a152-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



