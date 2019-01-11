---
title: Тип ресурса office365ActivationsUserDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: f87a5b32b08466428f0f6f0246a4b8d4c20e97be
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877338"
---
# <a name="office365activationsuserdetail-resource-type"></a><span data-ttu-id="f2e38-103">Тип ресурса office365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="f2e38-103">office365ActivationsUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="f2e38-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="f2e38-104">Properties</span></span>

| <span data-ttu-id="f2e38-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="f2e38-105">Property</span></span>             | <span data-ttu-id="f2e38-106">Тип</span><span class="sxs-lookup"><span data-stu-id="f2e38-106">Type</span></span>                                     | <span data-ttu-id="f2e38-107">Описание</span><span class="sxs-lookup"><span data-stu-id="f2e38-107">Description</span></span>                              |
| :------------------- | :--------------------------------------- | ---------------------------------------- |
| <span data-ttu-id="f2e38-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f2e38-108">reportRefreshDate</span></span>    | <span data-ttu-id="f2e38-109">Date</span><span class="sxs-lookup"><span data-stu-id="f2e38-109">Date</span></span>                                     | <span data-ttu-id="f2e38-110">Последняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="f2e38-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="f2e38-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f2e38-111">userPrincipalName</span></span>    | <span data-ttu-id="f2e38-112">Строка</span><span class="sxs-lookup"><span data-stu-id="f2e38-112">String</span></span>                                   | <span data-ttu-id="f2e38-113">Основной имя пользователя (UPN) пользователя.</span><span class="sxs-lookup"><span data-stu-id="f2e38-113">The user principal name (UPN) of the user.</span></span> <span data-ttu-id="f2e38-114">Имя участника-пользователя — это имя для входа характерном для Интернета для пользователя на основании Интернета standard RFC 822.</span><span class="sxs-lookup"><span data-stu-id="f2e38-114">The UPN is an Internet-style login name for the user based on the Internet standard RFC 822.</span></span> <span data-ttu-id="f2e38-115">В соответствии с соглашением это сопоставление имен пользователей электронной почты.</span><span class="sxs-lookup"><span data-stu-id="f2e38-115">By convention, this should map to the user's email name.</span></span> <span data-ttu-id="f2e38-116">Общие имеет формат alias@domain, где должны быть представлены в семейство подтвержденным доменов из домена.</span><span class="sxs-lookup"><span data-stu-id="f2e38-116">The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains.</span></span> <span data-ttu-id="f2e38-117">Это свойство обязательно указывать при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="f2e38-117">This property is required when a user is created.</span></span> |
| <span data-ttu-id="f2e38-118">displayName</span><span class="sxs-lookup"><span data-stu-id="f2e38-118">displayName</span></span>          | <span data-ttu-id="f2e38-119">String</span><span class="sxs-lookup"><span data-stu-id="f2e38-119">String</span></span>                                   | <span data-ttu-id="f2e38-120">Имя пользователя, отображаемое в адресной книге.</span><span class="sxs-lookup"><span data-stu-id="f2e38-120">The name displayed in the address book for the user.</span></span> <span data-ttu-id="f2e38-121">Обычно это сочетание имени, отчества и фамилии пользователя.</span><span class="sxs-lookup"><span data-stu-id="f2e38-121">This is usually the combination of the user's first name, middle initial, and last name.</span></span> <span data-ttu-id="f2e38-122">Это свойство необходимо указывать при создании пользователя. Его невозможно удалить при обновлении.</span><span class="sxs-lookup"><span data-stu-id="f2e38-122">This property is required when a user is created and it cannot be cleared during updates.</span></span> |
| <span data-ttu-id="f2e38-123">userActivationCounts</span><span class="sxs-lookup"><span data-stu-id="f2e38-123">userActivationCounts</span></span> | <span data-ttu-id="f2e38-124">[userActivationCounts](../resources/useractivationcounts.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="f2e38-124">[userActivationCounts](../resources/useractivationcounts.md) collection</span></span> | <span data-ttu-id="f2e38-125">Новейшие активации пользователя счетчиков для всех платформ для всех типов назначенный продукта.</span><span class="sxs-lookup"><span data-stu-id="f2e38-125">The user's latest product activation counts on all the platforms for all the assigned product types.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f2e38-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f2e38-126">JSON representation</span></span>

<span data-ttu-id="f2e38-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f2e38-127">The following is a JSON representation of the resource.</span></span>

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
