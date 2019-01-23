---
title: Удаление groupPolicyDefinitionValue
description: Удаляет groupPolicyDefinitionValue.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 80c56473102792d754092ef71cf539f793fbc5f8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430850"
---
# <a name="delete-grouppolicydefinitionvalue"></a><span data-ttu-id="3e496-103">Удаление groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="3e496-103">Delete groupPolicyDefinitionValue</span></span>

> <span data-ttu-id="3e496-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3e496-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3e496-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e496-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3e496-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3e496-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e496-107">Удаляет [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md).</span><span class="sxs-lookup"><span data-stu-id="3e496-107">Deletes a [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3e496-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="3e496-108">Prerequisites</span></span>
<span data-ttu-id="3e496-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3e496-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3e496-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e496-111">Permission type</span></span>|<span data-ttu-id="3e496-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e496-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e496-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e496-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3e496-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e496-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3e496-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e496-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e496-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e496-116">Not supported.</span></span>|
|<span data-ttu-id="3e496-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3e496-117">Application</span></span>|<span data-ttu-id="3e496-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e496-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e496-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e496-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}
DELETE /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/definitionValue
```

## <a name="request-headers"></a><span data-ttu-id="3e496-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3e496-120">Request headers</span></span>
|<span data-ttu-id="3e496-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3e496-121">Header</span></span>|<span data-ttu-id="3e496-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3e496-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e496-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3e496-123">Authorization</span></span>|<span data-ttu-id="3e496-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3e496-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e496-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3e496-125">Accept</span></span>|<span data-ttu-id="3e496-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3e496-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e496-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3e496-127">Request body</span></span>
<span data-ttu-id="3e496-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3e496-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e496-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e496-129">Response</span></span>
<span data-ttu-id="3e496-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3e496-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3e496-131">Пример</span><span class="sxs-lookup"><span data-stu-id="3e496-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3e496-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e496-132">Request</span></span>
<span data-ttu-id="3e496-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e496-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}
```

### <a name="response"></a><span data-ttu-id="3e496-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e496-134">Response</span></span>
<span data-ttu-id="3e496-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3e496-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




