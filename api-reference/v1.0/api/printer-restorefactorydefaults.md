---
title: 'принтер: restoreFactoryDefaults'
description: Сброс параметров по умолчанию принтера.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 64b8db4477e79918e863b80da236e42afec83f76
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50518125"
---
# <a name="printer-restorefactorydefaults"></a><span data-ttu-id="c86e9-103">принтер: restoreFactoryDefaults</span><span class="sxs-lookup"><span data-stu-id="c86e9-103">printer: restoreFactoryDefaults</span></span>
<span data-ttu-id="c86e9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c86e9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="c86e9-105">Восстановление [параметров](../resources/printer.md)по умолчанию принтера до значений, заданных производителем.</span><span class="sxs-lookup"><span data-stu-id="c86e9-105">Restore a [printer](../resources/printer.md)'s default settings to the values specified by the manufacturer.</span></span>

## <a name="permissions"></a><span data-ttu-id="c86e9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c86e9-106">Permissions</span></span>
<span data-ttu-id="c86e9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c86e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c86e9-109">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="c86e9-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="c86e9-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="c86e9-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="c86e9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c86e9-111">Permission type</span></span> | <span data-ttu-id="c86e9-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c86e9-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="c86e9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c86e9-113">Delegated (work or school account)</span></span>| <span data-ttu-id="c86e9-114">Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="c86e9-114">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="c86e9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c86e9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c86e9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c86e9-116">Not Supported.</span></span>|
|<span data-ttu-id="c86e9-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c86e9-117">Application</span></span>| <span data-ttu-id="c86e9-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c86e9-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c86e9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c86e9-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/printers/{printerId}/restoreFactoryDefaults
```

## <a name="request-headers"></a><span data-ttu-id="c86e9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c86e9-120">Request headers</span></span>
|<span data-ttu-id="c86e9-121">Имя</span><span class="sxs-lookup"><span data-stu-id="c86e9-121">Name</span></span>|<span data-ttu-id="c86e9-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c86e9-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c86e9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c86e9-123">Authorization</span></span>|<span data-ttu-id="c86e9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c86e9-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c86e9-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c86e9-126">Request body</span></span>
<span data-ttu-id="c86e9-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c86e9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c86e9-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="c86e9-128">Response</span></span>

<span data-ttu-id="c86e9-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c86e9-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c86e9-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="c86e9-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c86e9-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c86e9-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "printer_restorefactorydefaults"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/printers/{printerId}/restoreFactoryDefaults
```


### <a name="response"></a><span data-ttu-id="c86e9-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="c86e9-133">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

