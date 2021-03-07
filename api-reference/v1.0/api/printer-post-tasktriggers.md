---
title: Создание printTaskTrigger
description: Создайте новый триггер задач на указанном принтере.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: e02a2b0ce73d11153a0f778f9b0eeb80d505421b
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50518128"
---
# <a name="create-printtasktrigger"></a><span data-ttu-id="a89e0-103">Создание printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="a89e0-103">Create printTaskTrigger</span></span>
<span data-ttu-id="a89e0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a89e0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="a89e0-105">Создайте новый [триггер задач](../resources/printtasktrigger.md) на указанном [принтере.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="a89e0-105">Create a new [task trigger](../resources/printtasktrigger.md) on the specified [printer](../resources/printer.md).</span></span> <span data-ttu-id="a89e0-106">В настоящее **время на** принтере может быть указан только один триггер задач, но в будущем это ограничение может быть удалено.</span><span class="sxs-lookup"><span data-stu-id="a89e0-106">Currently, only **one** task trigger can be specified per printer, but this limit may be removed in the future.</span></span> 

## <a name="permissions"></a><span data-ttu-id="a89e0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a89e0-107">Permissions</span></span>
<span data-ttu-id="a89e0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a89e0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="a89e0-110">Помимо следующих разрешений, клиент пользователя должен иметь активную подписку на универсальную печать.</span><span class="sxs-lookup"><span data-stu-id="a89e0-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span> <span data-ttu-id="a89e0-111">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="a89e0-111">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="a89e0-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a89e0-112">Permission type</span></span> | <span data-ttu-id="a89e0-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a89e0-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="a89e0-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a89e0-114">Delegated (work or school account)</span></span>| <span data-ttu-id="a89e0-115">Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="a89e0-115">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="a89e0-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a89e0-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a89e0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a89e0-117">Not Supported.</span></span>|
|<span data-ttu-id="a89e0-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="a89e0-118">Application</span></span>|<span data-ttu-id="a89e0-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a89e0-119">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a89e0-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a89e0-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/printers/{printerId}/taskTriggers
```

## <a name="request-headers"></a><span data-ttu-id="a89e0-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a89e0-121">Request headers</span></span>
|<span data-ttu-id="a89e0-122">Имя</span><span class="sxs-lookup"><span data-stu-id="a89e0-122">Name</span></span>|<span data-ttu-id="a89e0-123">Описание</span><span class="sxs-lookup"><span data-stu-id="a89e0-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a89e0-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a89e0-124">Authorization</span></span>|<span data-ttu-id="a89e0-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a89e0-p104">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a89e0-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a89e0-127">Content-Type</span></span>|<span data-ttu-id="a89e0-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a89e0-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a89e0-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a89e0-130">Request body</span></span>
<span data-ttu-id="a89e0-131">В теле запроса подарйте JSON-представление [объекта printTaskTrigger.](../resources/printtasktrigger.md)</span><span class="sxs-lookup"><span data-stu-id="a89e0-131">In the request body, supply a JSON representation of a [printTaskTrigger](../resources/printtasktrigger.md) object.</span></span> <span data-ttu-id="a89e0-132">Поставляем ссылку на [печатьTaskDefinition](../resources/printtaskdefinition.md) с помощью `@odata.bind` формата, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="a89e0-132">Supply a reference to a [printTaskDefinition](../resources/printtaskdefinition.md) by using the `@odata.bind` format, as shown in the following example.</span></span>

## <a name="response"></a><span data-ttu-id="a89e0-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="a89e0-133">Response</span></span>
<span data-ttu-id="a89e0-134">В случае успешной работы этот метод возвращает код отклика и `201 Created` [печатьTaskTrigger](../resources/printtasktrigger.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a89e0-134">If successful, this method returns a `201 Created` response code and a [printTaskTrigger](../resources/printtasktrigger.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a89e0-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="a89e0-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a89e0-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="a89e0-136">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_printtasktrigger_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/printers/{printerId}/taskTriggers
Content-Type: application/json
Content-length: 80

{
  "event": "jobStarted",
  "definition@odata.bind": "https://graph.microsoft.com/v1.0/print/taskDefinitions/{taskDefinitionId}"
}
```


### <a name="response"></a><span data-ttu-id="a89e0-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="a89e0-137">Response</span></span>
<span data-ttu-id="a89e0-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a89e0-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskTrigger"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.context": "https://graph.print.microsoft.com/v1.0/$metadata#Collection(Microsoft.Graph.PrintTaskTrigger)",
  "id": "b6a843ca-e60e-4e20-a222-a58d85eead6d",
  "event": "jobStarted"
}
```

