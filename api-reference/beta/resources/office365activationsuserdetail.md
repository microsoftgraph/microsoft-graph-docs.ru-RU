---
title: Тип ресурса office365ActivationsUserDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 45219f7666d4432bcdb2b409491338b94650a726
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522479"
---
# <a name="office365activationsuserdetail-resource-type"></a><span data-ttu-id="2cb7b-103">Тип ресурса office365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="2cb7b-103">office365ActivationsUserDetail resource type</span></span>

<span data-ttu-id="2cb7b-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2cb7b-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="2cb7b-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="2cb7b-105">Properties</span></span>

| <span data-ttu-id="2cb7b-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="2cb7b-106">Property</span></span>             | <span data-ttu-id="2cb7b-107">Тип</span><span class="sxs-lookup"><span data-stu-id="2cb7b-107">Type</span></span>                                     | <span data-ttu-id="2cb7b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="2cb7b-108">Description</span></span>                              |
| :------------------- | :--------------------------------------- | ---------------------------------------- |
| <span data-ttu-id="2cb7b-109">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="2cb7b-109">reportRefreshDate</span></span>    | <span data-ttu-id="2cb7b-110">Дата</span><span class="sxs-lookup"><span data-stu-id="2cb7b-110">Date</span></span>                                     | <span data-ttu-id="2cb7b-111">Самая поздняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="2cb7b-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="2cb7b-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2cb7b-112">userPrincipalName</span></span>    | <span data-ttu-id="2cb7b-113">String</span><span class="sxs-lookup"><span data-stu-id="2cb7b-113">String</span></span>                                   | <span data-ttu-id="2cb7b-114">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="2cb7b-114">The user principal name (UPN) of the user.</span></span> <span data-ttu-id="2cb7b-115">Это имя для входа через Интернет по стандарту RFC 822.</span><span class="sxs-lookup"><span data-stu-id="2cb7b-115">The UPN is an Internet-style login name for the user based on the Internet standard RFC 822.</span></span> <span data-ttu-id="2cb7b-116">В соответствии с соглашением оно должно указывать на имя пользователя для электронной почты.</span><span class="sxs-lookup"><span data-stu-id="2cb7b-116">By convention, this should map to the user's email name.</span></span> <span data-ttu-id="2cb7b-117">Общий формат: псевдоним@домен. При этом домен должен входить в коллекцию проверенных доменов клиента.</span><span class="sxs-lookup"><span data-stu-id="2cb7b-117">The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains.</span></span> <span data-ttu-id="2cb7b-118">Это свойство обязательно указывать при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="2cb7b-118">This property is required when a user is created.</span></span> |
| <span data-ttu-id="2cb7b-119">displayName</span><span class="sxs-lookup"><span data-stu-id="2cb7b-119">displayName</span></span>          | <span data-ttu-id="2cb7b-120">Строка</span><span class="sxs-lookup"><span data-stu-id="2cb7b-120">String</span></span>                                   | <span data-ttu-id="2cb7b-121">Имя пользователя, отображаемое в адресной книге.</span><span class="sxs-lookup"><span data-stu-id="2cb7b-121">The name displayed in the address book for the user.</span></span> <span data-ttu-id="2cb7b-122">Обычно это сочетание имени, отчества и фамилии пользователя.</span><span class="sxs-lookup"><span data-stu-id="2cb7b-122">This is usually the combination of the user's first name, middle initial, and last name.</span></span> <span data-ttu-id="2cb7b-123">Это свойство необходимо указывать при создании пользователя. Его невозможно удалить при обновлении.</span><span class="sxs-lookup"><span data-stu-id="2cb7b-123">This property is required when a user is created and it cannot be cleared during updates.</span></span> |
| <span data-ttu-id="2cb7b-124">усерактиватионкаунтс</span><span class="sxs-lookup"><span data-stu-id="2cb7b-124">userActivationCounts</span></span> | <span data-ttu-id="2cb7b-125">Коллекция [усерактиватионкаунтс](../resources/useractivationcounts.md)</span><span class="sxs-lookup"><span data-stu-id="2cb7b-125">[userActivationCounts](../resources/useractivationcounts.md) collection</span></span> | <span data-ttu-id="2cb7b-126">Последние числа активаций на всех платформах для всех типов назначенных продуктов пользователя.</span><span class="sxs-lookup"><span data-stu-id="2cb7b-126">The user's latest product activation counts on all the platforms for all the assigned product types.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2cb7b-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2cb7b-127">JSON representation</span></span>

<span data-ttu-id="2cb7b-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2cb7b-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActivationsUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "userActivationCounts": [{"@odata.type":"microsoft.graph.userActivationCounts"}]
}
```
