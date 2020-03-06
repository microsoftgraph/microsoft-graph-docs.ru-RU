---
title: Обновление фотографии команды
description: Вы можете обновить фотографию (изображение) для команды.
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 26a0852df065e983de3e926bac06a751e9cc083f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452556"
---
# <a name="update-team-photo"></a><span data-ttu-id="a373d-103">Обновление фотографии команды</span><span class="sxs-lookup"><span data-stu-id="a373d-103">Update team photo</span></span>

<span data-ttu-id="a373d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a373d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a373d-105">Вы можете обновить фотографию (изображение) для команды.</span><span class="sxs-lookup"><span data-stu-id="a373d-105">Update the photo (picture) for a team.</span></span> <span data-ttu-id="a373d-106">Поддерживаемые размеры фотографий в формате HD для Office 365: 48 x 48, 64 x 64, 96 x 96, 120 x 120, 240 x 240, 360 x 360, 432 x 432, 504 x 504 и 648 x 648.</span><span class="sxs-lookup"><span data-stu-id="a373d-106">The following are the supported sizes of HD photos in Office 365: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648 pixels.</span></span> <span data-ttu-id="a373d-107">Фотографии, хранящиеся в Azure Active Directory, могут быть любого размера.</span><span class="sxs-lookup"><span data-stu-id="a373d-107">Photos can be any dimension if they are stored in Azure Active Directory.</span></span>

> [!Note]
> <span data-ttu-id="a373d-108">Общий размер запроса не должен превышать 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="a373d-108">There is a limit of 4 MB on the total size of the request.</span></span> <span data-ttu-id="a373d-109">Таким образом, размер фотографии составит менее 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="a373d-109">This limits the photo size to less than 4 MB.</span></span>

## <a name="permissions"></a><span data-ttu-id="a373d-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a373d-110">Permissions</span></span>

<span data-ttu-id="a373d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a373d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a373d-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a373d-113">Permission type</span></span>      | <span data-ttu-id="a373d-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a373d-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a373d-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a373d-115">Delegated (work or school account)</span></span> | <span data-ttu-id="a373d-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a373d-116">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a373d-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a373d-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a373d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a373d-118">Not supported.</span></span>    |
|<span data-ttu-id="a373d-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a373d-119">Application</span></span> | <span data-ttu-id="a373d-120">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a373d-120">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a373d-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a373d-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}-->

```http
PUT /beta/teams/{id}/photo
```

## <a name="request-headers"></a><span data-ttu-id="a373d-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a373d-122">Request headers</span></span>

| <span data-ttu-id="a373d-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a373d-123">Header</span></span>        | <span data-ttu-id="a373d-124">Значение</span><span class="sxs-lookup"><span data-stu-id="a373d-124">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="a373d-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a373d-125">Authorization</span></span> | <span data-ttu-id="a373d-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a373d-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a373d-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a373d-128">Content-type</span></span> | <span data-ttu-id="a373d-p105">image/jpeg. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a373d-p105">image/jpeg. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a373d-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a373d-131">Request body</span></span>

<span data-ttu-id="a373d-132">В текст запроса нужно включить двоичные данные фотографии.</span><span class="sxs-lookup"><span data-stu-id="a373d-132">In the request body, include the binary data of the photo.</span></span>

## <a name="response"></a><span data-ttu-id="a373d-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="a373d-133">Response</span></span>

<span data-ttu-id="a373d-134">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="a373d-134">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a373d-135">Пример</span><span class="sxs-lookup"><span data-stu-id="a373d-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="a373d-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="a373d-136">Request</span></span>

<span data-ttu-id="a373d-137">Ниже приведен пример запроса на обновление фотографии команды.</span><span class="sxs-lookup"><span data-stu-id="a373d-137">Here is an example of the request to update a team photo.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "update_team_photo"
}-->
```http
PUT https://graph.microsoft.com/beta/teams/{id}/photo
Content-type: image/jpeg

{
  <Binary data for the image>
}
```

### <a name="response"></a><span data-ttu-id="a373d-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="a373d-138">Response</span></span> 

<span data-ttu-id="a373d-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a373d-139">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update team photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
