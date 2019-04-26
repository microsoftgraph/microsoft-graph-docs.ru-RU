---
title: Удаление соглашения
description: Удаление объекта соглашения.
localization_priority: Normal
ms.openlocfilehash: 3d809383d8141ba038bcfe86788ef3016077d8e2
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322749"
---
# <a name="delete-agreement"></a><span data-ttu-id="5118a-103">Удаление соглашения</span><span class="sxs-lookup"><span data-stu-id="5118a-103">Delete agreement</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5118a-104">Удаление объекта [соглашения](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="5118a-104">Delete an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5118a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5118a-105">Permissions</span></span>
<span data-ttu-id="5118a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5118a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5118a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5118a-108">Permission type</span></span>                        | <span data-ttu-id="5118a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5118a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5118a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5118a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5118a-111">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5118a-111">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="5118a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5118a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5118a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5118a-113">Not supported.</span></span> |
|<span data-ttu-id="5118a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5118a-114">Application</span></span>                            | <span data-ttu-id="5118a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5118a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5118a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5118a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /agreements/<id>
```
## <a name="request-headers"></a><span data-ttu-id="5118a-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5118a-117">Request headers</span></span>
| <span data-ttu-id="5118a-118">Имя</span><span class="sxs-lookup"><span data-stu-id="5118a-118">Name</span></span>         | <span data-ttu-id="5118a-119">Тип</span><span class="sxs-lookup"><span data-stu-id="5118a-119">Type</span></span>        | <span data-ttu-id="5118a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5118a-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="5118a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5118a-121">Authorization</span></span> | <span data-ttu-id="5118a-122">string</span><span class="sxs-lookup"><span data-stu-id="5118a-122">string</span></span> | <span data-ttu-id="5118a-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5118a-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5118a-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5118a-125">Request body</span></span>
<span data-ttu-id="5118a-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5118a-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="5118a-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="5118a-127">Response</span></span>
<span data-ttu-id="5118a-p103">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5118a-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5118a-130">Пример</span><span class="sxs-lookup"><span data-stu-id="5118a-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5118a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="5118a-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_agreement"
}-->
```http
DELETE https://graph.microsoft.com/beta/agreements/<id>
```
##### <a name="response"></a><span data-ttu-id="5118a-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="5118a-132">Response</span></span>
><span data-ttu-id="5118a-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5118a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
