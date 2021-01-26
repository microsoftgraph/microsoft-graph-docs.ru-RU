---
title: Тип ресурса office365ActivationsUserDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: f1bb61fa4b740c212918ee8e4794ce79ffabafe7
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980747"
---
# <a name="office365activationsuserdetail-resource-type"></a><span data-ttu-id="edcaa-103">Тип ресурса office365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="edcaa-103">office365ActivationsUserDetail resource type</span></span>

<span data-ttu-id="edcaa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="edcaa-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="edcaa-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="edcaa-105">Properties</span></span>

| <span data-ttu-id="edcaa-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="edcaa-106">Property</span></span>             | <span data-ttu-id="edcaa-107">Тип</span><span class="sxs-lookup"><span data-stu-id="edcaa-107">Type</span></span>                                     | <span data-ttu-id="edcaa-108">Описание</span><span class="sxs-lookup"><span data-stu-id="edcaa-108">Description</span></span>                              |
| :------------------- | :--------------------------------------- | ---------------------------------------- |
| <span data-ttu-id="edcaa-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="edcaa-109">reportRefreshDate</span></span>    | <span data-ttu-id="edcaa-110">Дата</span><span class="sxs-lookup"><span data-stu-id="edcaa-110">Date</span></span>                                     | <span data-ttu-id="edcaa-111">Последняя дата содержимого.</span><span class="sxs-lookup"><span data-stu-id="edcaa-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="edcaa-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="edcaa-112">userPrincipalName</span></span>    | <span data-ttu-id="edcaa-113">String</span><span class="sxs-lookup"><span data-stu-id="edcaa-113">String</span></span>                                   | <span data-ttu-id="edcaa-114">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="edcaa-114">The user principal name (UPN) of the user.</span></span> <span data-ttu-id="edcaa-115">Это имя для входа через Интернет по стандарту RFC 822.</span><span class="sxs-lookup"><span data-stu-id="edcaa-115">The UPN is an Internet-style login name for the user based on the Internet standard RFC 822.</span></span> <span data-ttu-id="edcaa-116">В соответствии с соглашением оно должно указывать на имя пользователя для электронной почты.</span><span class="sxs-lookup"><span data-stu-id="edcaa-116">By convention, this should map to the user's email name.</span></span> <span data-ttu-id="edcaa-117">Общий формат: псевдоним@домен. При этом домен должен входить в коллекцию проверенных доменов клиента.</span><span class="sxs-lookup"><span data-stu-id="edcaa-117">The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains.</span></span> <span data-ttu-id="edcaa-118">Это свойство обязательно указывать при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="edcaa-118">This property is required when a user is created.</span></span> |
| <span data-ttu-id="edcaa-119">displayName</span><span class="sxs-lookup"><span data-stu-id="edcaa-119">displayName</span></span>          | <span data-ttu-id="edcaa-120">String</span><span class="sxs-lookup"><span data-stu-id="edcaa-120">String</span></span>                                   | <span data-ttu-id="edcaa-121">Имя пользователя, отображаемое в адресной книге.</span><span class="sxs-lookup"><span data-stu-id="edcaa-121">The name displayed in the address book for the user.</span></span> <span data-ttu-id="edcaa-122">Обычно это сочетание имени, отчества и фамилии пользователя.</span><span class="sxs-lookup"><span data-stu-id="edcaa-122">This is usually the combination of the user's first name, middle initial, and last name.</span></span> <span data-ttu-id="edcaa-123">Это свойство необходимо указывать при создании пользователя. Его невозможно удалить при обновлении.</span><span class="sxs-lookup"><span data-stu-id="edcaa-123">This property is required when a user is created and it cannot be cleared during updates.</span></span> |
| <span data-ttu-id="edcaa-124">userActivationCounts</span><span class="sxs-lookup"><span data-stu-id="edcaa-124">userActivationCounts</span></span> | <span data-ttu-id="edcaa-125">[Коллекция userActivationCounts](../resources/useractivationcounts.md)</span><span class="sxs-lookup"><span data-stu-id="edcaa-125">[userActivationCounts](../resources/useractivationcounts.md) collection</span></span> | <span data-ttu-id="edcaa-126">Последняя активация продукта пользователя учитывается на всех платформах для всех типов продуктов.</span><span class="sxs-lookup"><span data-stu-id="edcaa-126">The user's latest product activation counts on all the platforms for all the assigned product types.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="edcaa-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="edcaa-127">JSON representation</span></span>

<span data-ttu-id="edcaa-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="edcaa-128">The following is a JSON representation of the resource.</span></span>

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


