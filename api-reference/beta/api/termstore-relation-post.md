---
title: Создание отношения
description: Создание объекта связи.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: b8323a8b2b5cc9ad9547182d9db8bdeba17934f7
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539419"
---
# <a name="create-relation"></a><span data-ttu-id="d9668-103">Создание отношения</span><span class="sxs-lookup"><span data-stu-id="d9668-103">Create relation</span></span>
<span data-ttu-id="d9668-104">Пространство имен: Microsoft. Graph. банка</span><span class="sxs-lookup"><span data-stu-id="d9668-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9668-105">Создание объекта [связи](../resources/termstore-relation.md) .</span><span class="sxs-lookup"><span data-stu-id="d9668-105">Create a new [relation](../resources/termstore-relation.md) object.</span></span> <span data-ttu-id="d9668-106">Они используются для создания закрепленных и ресуед связей между терминами или между термином и набором.</span><span class="sxs-lookup"><span data-stu-id="d9668-106">These are used to create pinned and resued relations between terms or between a term and set.</span></span> <span data-ttu-id="d9668-107">При создании закрепленного/повторно используемого термина между термином и set значение Фромтерм в тексте POST должно иметь значение null.</span><span class="sxs-lookup"><span data-stu-id="d9668-107">When creating a pinned/reused term between term and set then fromTerm in the post body must be null.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9668-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d9668-108">Permissions</span></span>
<span data-ttu-id="d9668-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9668-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9668-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d9668-111">Permission type</span></span>|<span data-ttu-id="d9668-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d9668-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9668-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d9668-113">Delegated (work or school account)</span></span> |<span data-ttu-id="d9668-114">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9668-114">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="d9668-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d9668-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9668-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9668-116">Not supported.</span></span>    |
|<span data-ttu-id="d9668-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d9668-117">Application</span></span> | <span data-ttu-id="d9668-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9668-118">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="d9668-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d9668-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /termStore/sets/{setId}/terms/{termId}/relations
```

## <a name="request-headers"></a><span data-ttu-id="d9668-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d9668-120">Request headers</span></span>
|<span data-ttu-id="d9668-121">Имя</span><span class="sxs-lookup"><span data-stu-id="d9668-121">Name</span></span>|<span data-ttu-id="d9668-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d9668-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d9668-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d9668-123">Authorization</span></span>|<span data-ttu-id="d9668-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d9668-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d9668-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d9668-126">Content-Type</span></span>|<span data-ttu-id="d9668-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d9668-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9668-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d9668-129">Request body</span></span>
<span data-ttu-id="d9668-130">В тексте запроса добавьте представление объекта [relation](../resources/termstore-relation.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d9668-130">In the request body, supply a JSON representation of the [relation](../resources/termstore-relation.md) object.</span></span>

<span data-ttu-id="d9668-131">В следующей таблице приведены свойства, необходимые при создании [отношения](../resources/termstore-relation.md).</span><span class="sxs-lookup"><span data-stu-id="d9668-131">The following table shows the properties that are required when you create the [relation](../resources/termstore-relation.md).</span></span>

|<span data-ttu-id="d9668-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="d9668-132">Property</span></span>|<span data-ttu-id="d9668-133">Тип</span><span class="sxs-lookup"><span data-stu-id="d9668-133">Type</span></span>|<span data-ttu-id="d9668-134">Описание</span><span class="sxs-lookup"><span data-stu-id="d9668-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9668-135">Отношение</span><span class="sxs-lookup"><span data-stu-id="d9668-135">relationship</span></span>|<span data-ttu-id="d9668-136">релатионтипе</span><span class="sxs-lookup"><span data-stu-id="d9668-136">relationType</span></span>|<span data-ttu-id="d9668-137">Тип создаваемого отношения.</span><span class="sxs-lookup"><span data-stu-id="d9668-137">Type of relation to be created.</span></span> <span data-ttu-id="d9668-138">Возможные значения: `pin`, `reuse`.</span><span class="sxs-lookup"><span data-stu-id="d9668-138">Possible values are: `pin`, `reuse`.</span></span>|
|<span data-ttu-id="d9668-139">set</span><span class="sxs-lookup"><span data-stu-id="d9668-139">set</span></span>| [<span data-ttu-id="d9668-140">Microsoft. Graph. банка. Set</span><span class="sxs-lookup"><span data-stu-id="d9668-140">microsoft.graph.termstore.set</span></span>](../resources/termstore-set.md)| <span data-ttu-id="d9668-141">Набор, в котором необходимо создать связь.</span><span class="sxs-lookup"><span data-stu-id="d9668-141">The set where the relationship needs to be created.</span></span>
|<span data-ttu-id="d9668-142">фромтерм</span><span class="sxs-lookup"><span data-stu-id="d9668-142">fromTerm</span></span>| [<span data-ttu-id="d9668-143">Microsoft. Graph. Банк. Term</span><span class="sxs-lookup"><span data-stu-id="d9668-143">microsoft.graph.termstore.term</span></span>](../resources/termstore-term.md) | <span data-ttu-id="d9668-144">Термин, с которым необходимо создать связь.</span><span class="sxs-lookup"><span data-stu-id="d9668-144">The term with which the relationship needs to be created.</span></span>



## <a name="response"></a><span data-ttu-id="d9668-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9668-145">Response</span></span>

<span data-ttu-id="d9668-146">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [relation](../resources/termstore-relation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d9668-146">If successful, this method returns a `201 Created` response code and a [relation](../resources/termstore-relation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d9668-147">Примеры</span><span class="sxs-lookup"><span data-stu-id="d9668-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d9668-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="d9668-148">Request</span></span>

``` http
POST https://graph.microsoft.com/beta/termStore/sets/{setId}/terms/{termId}/relations
Content-Type: application/json
Content-length: 89

{
  "@odata.type": "#microsoft.graph.termStore.relation",
  "relationship": "pin",
  "fromTerm" : {
    "id" : "b49f64b3-4722-4336-9a5c-56c326b344d4"
  },
  "set" : {
    "id": "95e553ae-a91a-4670-a139-67a6cea285b3"
  }
}
```


### <a name="response"></a><span data-ttu-id="d9668-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9668-149">Response</span></span>
<span data-ttu-id="d9668-150">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d9668-150">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termstore.relation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.termStore.relation",
  "id": "052c749c-749c-052c-9c74-2c059c742c05",
  "relationship": "pin",
  "fromTerm" : {
      "id" : "b49f64b3-4722-4336-9a5c-56c326b344d4"
  },
  "toTerm" : {
      "id" : "226e8ee3-f4b6-49d7-92d5-ec9d5475eec5"
  },
  "set" : {
      "id" : "95e553ae-a91a-4670-a139-67a6cea285b3"
  }
}
```

[microsoft.graph.termStore.set]: ../resources/termstore-set.md
[microsoft.graph.termStore.term]: ../resources/termstore-term.md
[microsoft.graph.termStore.relation]: ../resources/termstore-relation.md


<!--
{
  "type": "#page.annotation",
  "description": "Create a pinned term entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Pinned term",
  "suppressions": [
  ]
}
-->
