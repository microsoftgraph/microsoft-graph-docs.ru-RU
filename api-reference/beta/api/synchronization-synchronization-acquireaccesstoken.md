---
title: 'Синхронизация: Аккуиреакцесстокен'
description: Получение маркера доступа OAuth для авторизации службы подготовки Azure AD для подготовки пользователей в приложении
author: ArvindHarinder1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c31da95c5da037717b1c10fc9908e41cc91392ea
ms.sourcegitcommit: 79267b6d78c3510ef609953c5a664e692794caaa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/21/2020
ms.locfileid: "45197459"
---
# <a name="acquireaccesstoken"></a><span data-ttu-id="d9637-103">аккуиреакцесстокен</span><span class="sxs-lookup"><span data-stu-id="d9637-103">acquireAccessToken</span></span>
<span data-ttu-id="d9637-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9637-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d9637-105">Получите маркер доступа OAuth, чтобы авторизовать службу подготовки Azure AD для подготовки пользователей в приложении.</span><span class="sxs-lookup"><span data-stu-id="d9637-105">Acquire an OAuth Access token to authorize the Azure AD provisioning service to provision users into an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9637-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d9637-106">Permissions</span></span>
<span data-ttu-id="d9637-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9637-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9637-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d9637-109">Permission type</span></span>|<span data-ttu-id="d9637-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d9637-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9637-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d9637-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d9637-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9637-112">Directory.ReadWrite.All</span></span>|
|<span data-ttu-id="d9637-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d9637-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9637-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9637-114">Not supported.</span></span>|
|<span data-ttu-id="d9637-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d9637-115">Application</span></span>|<span data-ttu-id="d9637-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9637-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9637-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d9637-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /applications/{applicationsId}/synchronization/acquireAccessToken
POST /servicePrincipals/{servicePrincipalsId}/synchronization/acquireAccessToken
```

## <a name="request-headers"></a><span data-ttu-id="d9637-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d9637-118">Request headers</span></span>
|<span data-ttu-id="d9637-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d9637-119">Name</span></span>|<span data-ttu-id="d9637-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d9637-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d9637-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d9637-121">Authorization</span></span>|<span data-ttu-id="d9637-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d9637-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d9637-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d9637-124">Content-Type</span></span>|<span data-ttu-id="d9637-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d9637-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9637-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d9637-127">Request body</span></span>
<span data-ttu-id="d9637-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d9637-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d9637-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="d9637-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d9637-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="d9637-130">Parameter</span></span>|<span data-ttu-id="d9637-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d9637-131">Type</span></span>|<span data-ttu-id="d9637-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d9637-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9637-133">записей</span><span class="sxs-lookup"><span data-stu-id="d9637-133">credentials</span></span>|<span data-ttu-id="d9637-134">Коллекция [синчронизатионсекреткэйстрингвалуепаир](../resources/synchronization-secretkeystringvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="d9637-134">[synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md) collection</span></span>|<span data-ttu-id="d9637-135">Представляет одно секретное значение.</span><span class="sxs-lookup"><span data-stu-id="d9637-135">Represents a single secret value.</span></span>|



## <a name="response"></a><span data-ttu-id="d9637-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="d9637-136">Response</span></span>

<span data-ttu-id="d9637-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d9637-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="d9637-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="d9637-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d9637-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="d9637-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronization_acquireaccesstoken"
}
-->
``` http
POST https://graph.microsoft.com/beta/applications/{applicationsId}/synchronization/acquireAccessToken
Content-Type: application/json
Content-length: 123

{
  "credentials": [
    {
      "@odata.type": "microsoft.graph.synchronizationSecretKeyStringValuePair"
    }
  ]
}
```


### <a name="response"></a><span data-ttu-id="d9637-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9637-140">Response</span></span>
<span data-ttu-id="d9637-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d9637-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
