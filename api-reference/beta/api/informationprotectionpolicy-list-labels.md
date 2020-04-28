---
title: 'Информатионпротектионлабел: Листлабелс'
description: Получение списка меток защиты информации.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 94b47a2bac3e3000af5123bf2a7b4dd88c43e0cf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446340"
---
# <a name="informationprotectionlabel-listlabels"></a><span data-ttu-id="9ef54-103">Информатионпротектионлабел: Листлабелс</span><span class="sxs-lookup"><span data-stu-id="9ef54-103">informationProtectionLabel: listLabels</span></span>

<span data-ttu-id="9ef54-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ef54-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ef54-105">Получение набора [меток защиты информации](../resources/informationprotectionlabel.md) , доступных пользователю или организации.</span><span class="sxs-lookup"><span data-stu-id="9ef54-105">Get a collection of [information protection labels](../resources/informationprotectionlabel.md) available to the user or to the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ef54-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9ef54-106">Permissions</span></span>

<span data-ttu-id="9ef54-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ef54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9ef54-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ef54-109">Permission type</span></span>                        | <span data-ttu-id="9ef54-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ef54-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="9ef54-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ef54-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9ef54-112">Информатионпротектионполици. Read</span><span class="sxs-lookup"><span data-stu-id="9ef54-112">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="9ef54-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ef54-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ef54-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ef54-114">Not supported.</span></span>                              |
| <span data-ttu-id="9ef54-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9ef54-115">Application</span></span>                            | <span data-ttu-id="9ef54-116">Информатионпротектионполици. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="9ef54-116">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="9ef54-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ef54-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/informationprotection/policy/labels
GET /informationprotection/policy/labels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9ef54-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9ef54-118">Optional query parameters</span></span>

<span data-ttu-id="9ef54-119">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9ef54-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="9ef54-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="9ef54-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9ef54-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9ef54-121">Request headers</span></span>

| <span data-ttu-id="9ef54-122">Имя</span><span class="sxs-lookup"><span data-stu-id="9ef54-122">Name</span></span>          | <span data-ttu-id="9ef54-123">Описание</span><span class="sxs-lookup"><span data-stu-id="9ef54-123">Description</span></span>                                                                                                                                                                       |
| :------------ | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="9ef54-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9ef54-124">Authorization</span></span> | <span data-ttu-id="9ef54-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ef54-p103">Bearer {token}. Required.</span></span>                                                                                                                                                         |
| <span data-ttu-id="9ef54-127">User — Agent</span><span class="sxs-lookup"><span data-stu-id="9ef54-127">User-Agent</span></span>    | <span data-ttu-id="9ef54-128">Описывает имя и версию вызывающего приложения.</span><span class="sxs-lookup"><span data-stu-id="9ef54-128">Describes the name and version of the calling application.</span></span> <span data-ttu-id="9ef54-129">Подробные сведения отображаются в Azure Information Protection Analytics.</span><span class="sxs-lookup"><span data-stu-id="9ef54-129">Details will surface in Azure Information Protection Analytics.</span></span> <span data-ttu-id="9ef54-130">Рекомендуемый формат — ApplicationName/Version.</span><span class="sxs-lookup"><span data-stu-id="9ef54-130">Suggested format is ApplicationName/Version.</span></span> <span data-ttu-id="9ef54-131">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="9ef54-131">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9ef54-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9ef54-132">Request body</span></span>

<span data-ttu-id="9ef54-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9ef54-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ef54-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="9ef54-134">Response</span></span>

<span data-ttu-id="9ef54-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [информатионпротектионлабел](../resources/informationprotectionlabel.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9ef54-135">If successful, this method returns a `200 OK` response code and a collection of [informationProtectionLabel](../resources/informationprotectionlabel.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9ef54-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="9ef54-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9ef54-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ef54-137">Request</span></span>

<span data-ttu-id="9ef54-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9ef54-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9ef54-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ef54-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_labels"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/informationprotection/policy/labels
```
# <a name="c"></a>[<span data-ttu-id="9ef54-140">C#</span><span class="sxs-lookup"><span data-stu-id="9ef54-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-labels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9ef54-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ef54-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-labels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9ef54-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ef54-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-labels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9ef54-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ef54-143">Response</span></span>

<span data-ttu-id="9ef54-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9ef54-144">The following is an example of the response.</span></span>

> <span data-ttu-id="9ef54-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9ef54-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.informationProtectionLabel",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
User-agent: ContosoLOBApp/1.0

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('1e36d926-d716-4197-ba86-a6e18eb910b9')/informationProtection/policy/labels",
  "value": [
      {
          "id": "3a80e051-487c-40d4-b491-73ad25d997e6",
          "name": "General",
          "description": "Consult Contoso data labeling policy for more details.",
          "color": "",
          "sensitivity": 1,
          "tooltip": "Data classified as Contoso General.",
          "isActive": true
      },
      {
          "id": "4662f9a3-dd50-4a20-b984-a7be82e0e79c",
          "name": "Confidential",
          "description": "Consult Contoso data labeling policy for more details.",
          "color": "",
          "sensitivity": 2,
          "tooltip": "Data classificed as Contoso Confidential.",
          "isActive": true
      },
      {
          "id": "4b18e8bb-b4a5-4695-85d0-8ae23ef27892",
          "name": "Highly Confidential",
          "description": "Consult Contoso data labeling policy for more details.",
          "color": "",
          "sensitivity": 3,
          "tooltip": "Data classified as Contoso Highly Confidential.",
          "isActive": true
      }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List labels",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
