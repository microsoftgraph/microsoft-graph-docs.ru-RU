---
title: Удаление printerShare
description: Удаление доли принтера (стереть связанный принтер). Это действие невозможно отменить. Если принтер будет снова открыт в будущем, пользователям Windows, которые ранее установили принтер, потребуется его обнаружить и повторно установить.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 5ca8d4e8c4dd0540d4ab585952aa82f6244cc6d2
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517368"
---
# <a name="delete-printershare"></a><span data-ttu-id="0e099-105">Удаление printerShare</span><span class="sxs-lookup"><span data-stu-id="0e099-105">Delete printerShare</span></span>
<span data-ttu-id="0e099-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e099-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="0e099-107">Удаление доли принтера (удалить связанный [принтер).](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="0e099-107">Delete a printer share (unshare the associated [printer](../resources/printer.md)).</span></span> <span data-ttu-id="0e099-108">Это действие невозможно отменить.</span><span class="sxs-lookup"><span data-stu-id="0e099-108">This action cannot be undone.</span></span> <span data-ttu-id="0e099-109">Если принтер [будет](../resources/printer.md) снова открыт в будущем, пользователям Windows, которые ранее установили принтер, потребуется его обнаружить и переустановить. [](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="0e099-109">If the [printer](../resources/printer.md) is shared again in the future, any Windows users who had previously installed the [printer](../resources/printer.md) will need to discover and reinstall it.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e099-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0e099-110">Permissions</span></span>
<span data-ttu-id="0e099-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e099-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="0e099-113">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="0e099-113">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="0e099-114">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="0e099-114">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="0e099-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0e099-115">Permission type</span></span> | <span data-ttu-id="0e099-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0e099-116">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="0e099-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0e099-117">Delegated (work or school account)</span></span>| <span data-ttu-id="0e099-118">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e099-118">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="0e099-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0e099-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e099-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e099-120">Not Supported.</span></span>|
|<span data-ttu-id="0e099-121">Приложение</span><span class="sxs-lookup"><span data-stu-id="0e099-121">Application</span></span>|<span data-ttu-id="0e099-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e099-122">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e099-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0e099-123">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /print/shares/{printerShareId}
```

## <a name="request-headers"></a><span data-ttu-id="0e099-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0e099-124">Request headers</span></span>
|<span data-ttu-id="0e099-125">Имя</span><span class="sxs-lookup"><span data-stu-id="0e099-125">Name</span></span>|<span data-ttu-id="0e099-126">Описание</span><span class="sxs-lookup"><span data-stu-id="0e099-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0e099-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0e099-127">Authorization</span></span>|<span data-ttu-id="0e099-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0e099-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e099-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0e099-130">Request body</span></span>
<span data-ttu-id="0e099-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0e099-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e099-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e099-132">Response</span></span>

<span data-ttu-id="0e099-p106">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0e099-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0e099-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="0e099-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0e099-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="0e099-136">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_printershare"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/print/shares/{printerShareId}
```


### <a name="response"></a><span data-ttu-id="0e099-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e099-137">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

