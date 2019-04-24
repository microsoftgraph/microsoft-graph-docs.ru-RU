---
title: Тип ресурса office365ActivationsUserDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: a3561768e36fc63c779e19a9aa05863dd9af9315
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32505496"
---
# <a name="office365activationsuserdetail-resource-type"></a><span data-ttu-id="dfcfe-103">Тип ресурса office365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="dfcfe-103">office365ActivationsUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="dfcfe-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="dfcfe-104">Properties</span></span>

| <span data-ttu-id="dfcfe-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="dfcfe-105">Property</span></span>             | <span data-ttu-id="dfcfe-106">Тип</span><span class="sxs-lookup"><span data-stu-id="dfcfe-106">Type</span></span>                                     | <span data-ttu-id="dfcfe-107">Описание</span><span class="sxs-lookup"><span data-stu-id="dfcfe-107">Description</span></span>                              |
| :------------------- | :--------------------------------------- | ---------------------------------------- |
| <span data-ttu-id="dfcfe-108">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="dfcfe-108">reportRefreshDate</span></span>    | <span data-ttu-id="dfcfe-109">Дата</span><span class="sxs-lookup"><span data-stu-id="dfcfe-109">Date</span></span>                                     | <span data-ttu-id="dfcfe-110">Самая поздняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="dfcfe-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="dfcfe-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="dfcfe-111">userPrincipalName</span></span>    | <span data-ttu-id="dfcfe-112">String</span><span class="sxs-lookup"><span data-stu-id="dfcfe-112">String</span></span>                                   | <span data-ttu-id="dfcfe-113">Имя участника-пользователя (UPN).</span><span class="sxs-lookup"><span data-stu-id="dfcfe-113">The user principal name (UPN) of the user.</span></span> <span data-ttu-id="dfcfe-114">UPN — это имя входа в стиле Интернета для пользователя на основе стандартного стандарта RFC 822.</span><span class="sxs-lookup"><span data-stu-id="dfcfe-114">The UPN is an Internet-style login name for the user based on the Internet standard RFC 822.</span></span> <span data-ttu-id="dfcfe-115">По соглашению он должен сопоставляться с именем электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="dfcfe-115">By convention, this should map to the user's email name.</span></span> <span data-ttu-id="dfcfe-116">Общий формат — псевдоним @ Domain, где домен должен присутствовать в коллекции проверенных доменов клиента.</span><span class="sxs-lookup"><span data-stu-id="dfcfe-116">The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains.</span></span> <span data-ttu-id="dfcfe-117">Это свойство обязательно указывать при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="dfcfe-117">This property is required when a user is created.</span></span> |
| <span data-ttu-id="dfcfe-118">displayName</span><span class="sxs-lookup"><span data-stu-id="dfcfe-118">displayName</span></span>          | <span data-ttu-id="dfcfe-119">String</span><span class="sxs-lookup"><span data-stu-id="dfcfe-119">String</span></span>                                   | <span data-ttu-id="dfcfe-120">Имя пользователя, отображаемое в адресной книге.</span><span class="sxs-lookup"><span data-stu-id="dfcfe-120">The name displayed in the address book for the user.</span></span> <span data-ttu-id="dfcfe-121">Обычно это сочетание имени, отчества и фамилии пользователя.</span><span class="sxs-lookup"><span data-stu-id="dfcfe-121">This is usually the combination of the user's first name, middle initial, and last name.</span></span> <span data-ttu-id="dfcfe-122">Это свойство необходимо указывать при создании пользователя. Его невозможно удалить при обновлении.</span><span class="sxs-lookup"><span data-stu-id="dfcfe-122">This property is required when a user is created and it cannot be cleared during updates.</span></span> |
| <span data-ttu-id="dfcfe-123">Усерактиватионкаунтс</span><span class="sxs-lookup"><span data-stu-id="dfcfe-123">userActivationCounts</span></span> | <span data-ttu-id="dfcfe-124">Коллекция [усерактиватионкаунтс](../resources/useractivationcounts.md)</span><span class="sxs-lookup"><span data-stu-id="dfcfe-124">[userActivationCounts](../resources/useractivationcounts.md) collection</span></span> | <span data-ttu-id="dfcfe-125">Последние числа активаций на всех платформах для всех типов назначенных продуктов пользователя.</span><span class="sxs-lookup"><span data-stu-id="dfcfe-125">The user's latest product activation counts on all the platforms for all the assigned product types.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="dfcfe-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dfcfe-126">JSON representation</span></span>

<span data-ttu-id="dfcfe-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dfcfe-127">The following is a JSON representation of the resource.</span></span>

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
