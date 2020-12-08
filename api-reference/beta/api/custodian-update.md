---
title: Обновление хранитель
description: Обновление свойств объекта хранитель.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: c9c58671dd2be9d97e9317cc0b268245402b44e5
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597734"
---
# <a name="update-custodian"></a><span data-ttu-id="3892f-103">Обновление хранитель</span><span class="sxs-lookup"><span data-stu-id="3892f-103">Update custodian</span></span>

<span data-ttu-id="3892f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3892f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3892f-105">Обновление свойств объекта [хранитель](../resources/custodian.md) .</span><span class="sxs-lookup"><span data-stu-id="3892f-105">Update the properties of a [custodian](../resources/custodian.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3892f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3892f-106">Permissions</span></span>

<span data-ttu-id="3892f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3892f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3892f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3892f-109">Permission type</span></span>|<span data-ttu-id="3892f-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3892f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3892f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3892f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3892f-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="3892f-112">User.Read</span></span>|
|<span data-ttu-id="3892f-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3892f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3892f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3892f-114">Not supported.</span></span>|
|<span data-ttu-id="3892f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3892f-115">Application</span></span>|<span data-ttu-id="3892f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3892f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3892f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3892f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}
```

## <a name="request-headers"></a><span data-ttu-id="3892f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3892f-118">Request headers</span></span>

|<span data-ttu-id="3892f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3892f-119">Name</span></span>|<span data-ttu-id="3892f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3892f-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3892f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3892f-121">Authorization</span></span>|<span data-ttu-id="3892f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3892f-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="3892f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3892f-124">Content-Type</span></span>|<span data-ttu-id="3892f-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3892f-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3892f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3892f-127">Request body</span></span>

<span data-ttu-id="3892f-128">В тексте запроса добавьте представление объекта [хранитель](../resources/custodian.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3892f-128">In the request body, supply a JSON representation of the [custodian](../resources/custodian.md) object.</span></span>

<span data-ttu-id="3892f-129">В следующей таблице приведены свойства объекта [хранитель](../resources/custodian.md) , которые можно изменить.</span><span class="sxs-lookup"><span data-stu-id="3892f-129">The following table lists the properties of a [custodian](../resources/custodian.md) object that can be modified.</span></span>

|<span data-ttu-id="3892f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3892f-130">Property</span></span>|<span data-ttu-id="3892f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3892f-131">Type</span></span>|<span data-ttu-id="3892f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3892f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3892f-133">апплихолдтосаурцес</span><span class="sxs-lookup"><span data-stu-id="3892f-133">applyHoldToSources</span></span>|<span data-ttu-id="3892f-134">Логический</span><span class="sxs-lookup"><span data-stu-id="3892f-134">Boolean</span></span>|<span data-ttu-id="3892f-135">Определяет, были ли источники хранитель сохранены во время создания.</span><span class="sxs-lookup"><span data-stu-id="3892f-135">Identifies whether a custodian's sources were placed on hold during creation.</span></span> <span data-ttu-id="3892f-136">Дополнительные сведения см. [в разделе помещение custodians на удержании](/microsoft-365/compliance/add-custodians-to-case#step-4-place-custodians-on-hold).</span><span class="sxs-lookup"><span data-stu-id="3892f-136">For details, see [Place custodians on hold](/microsoft-365/compliance/add-custodians-to-case#step-4-place-custodians-on-hold).</span></span>|

## <a name="response"></a><span data-ttu-id="3892f-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="3892f-137">Response</span></span>

<span data-ttu-id="3892f-138">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [хранитель](../resources/custodian.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3892f-138">If successful, this method returns a `200 OK` response code and an updated [custodian](../resources/custodian.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3892f-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="3892f-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3892f-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="3892f-140">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_custodian"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians/45454331323337443946343043464239
Content-Type: application/json
Content-length: 254

{
  "applyHoldToSources": "false",
}
```

### <a name="response"></a><span data-ttu-id="3892f-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="3892f-141">Response</span></span>

<span data-ttu-id="3892f-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3892f-142">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.custodian"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/$entity",
    "email": "AdeleV@contoso.com",
    "applyHoldToSources": false,
    "status": "active",
    "createdDateTime": "2020-10-30T20:59:54.9900703Z",
    "lastModifiedDateTime": "2020-10-30T21:01:34.1400013Z",
    "releasedDateTime": null,
    "acknowledgedDateTime": null,
    "id": "45454331323337443946343043464239",
    "displayName": "Adele Vance"
}
```
