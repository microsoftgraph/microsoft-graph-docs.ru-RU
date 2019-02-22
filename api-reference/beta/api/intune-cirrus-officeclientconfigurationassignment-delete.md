---
title: Удаление Оффицеклиентконфигуратионассигнмент
description: Удаляет объект Оффицеклиентконфигуратионассигнмент.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 49b4401887276957ecf220802ae67a3803497212
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151417"
---
# <a name="delete-officeclientconfigurationassignment"></a><span data-ttu-id="0ee20-103">Удаление Оффицеклиентконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="0ee20-103">Delete officeClientConfigurationAssignment</span></span>

> <span data-ttu-id="0ee20-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ee20-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ee20-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0ee20-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ee20-106">Удаляет объект [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="0ee20-106">Deletes a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0ee20-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0ee20-107">Prerequisites</span></span>
<span data-ttu-id="0ee20-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ee20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ee20-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ee20-110">Permission type</span></span>|<span data-ttu-id="0ee20-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ee20-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ee20-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ee20-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0ee20-113">\* \* TODO: определение областей \* \*</span><span class="sxs-lookup"><span data-stu-id="0ee20-113">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="0ee20-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ee20-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ee20-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ee20-115">Not supported.</span></span>|
|<span data-ttu-id="0ee20-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0ee20-116">Application</span></span>|<span data-ttu-id="0ee20-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ee20-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ee20-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ee20-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="0ee20-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0ee20-119">Request headers</span></span>
|<span data-ttu-id="0ee20-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0ee20-120">Header</span></span>|<span data-ttu-id="0ee20-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0ee20-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ee20-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0ee20-122">Authorization</span></span>|<span data-ttu-id="0ee20-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0ee20-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ee20-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0ee20-124">Accept</span></span>|<span data-ttu-id="0ee20-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0ee20-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ee20-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0ee20-126">Request body</span></span>
<span data-ttu-id="0ee20-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0ee20-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ee20-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ee20-128">Response</span></span>
<span data-ttu-id="0ee20-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0ee20-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0ee20-130">Пример</span><span class="sxs-lookup"><span data-stu-id="0ee20-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ee20-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ee20-131">Request</span></span>
<span data-ttu-id="0ee20-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0ee20-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="0ee20-133">Отклик
</span><span class="sxs-lookup"><span data-stu-id="0ee20-133">Response</span></span>
<span data-ttu-id="0ee20-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0ee20-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



