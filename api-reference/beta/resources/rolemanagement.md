---
title: Тип ресурса Ролеманажемент
description: Ресурс управления ролями RBAC
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: bd4e1eefeae819d37630a7faf4fbb1f6d1a5124c
ms.sourcegitcommit: 567d0420243765b4088bc8029306a517f92926fd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/16/2019
ms.locfileid: "36437820"
---
# <a name="rolemanagement-resource-type"></a><span data-ttu-id="ea17a-103">Тип ресурса Ролеманажемент</span><span class="sxs-lookup"><span data-stu-id="ea17a-103">roleManagement resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea17a-104">Объект управления ролями Microsoft 365 RBAC.</span><span class="sxs-lookup"><span data-stu-id="ea17a-104">Microsoft 365 RBAC role management entity.</span></span> <span data-ttu-id="ea17a-105">Предоставляет доступ к определениям ролей и назначениям ролей, предоставляемым поставщикам RBAC.</span><span class="sxs-lookup"><span data-stu-id="ea17a-105">Provides access to role definitions and role assignments surfaced from RBAC providers.</span></span> <span data-ttu-id="ea17a-106">В настоящее время поддерживается только поставщик каталогов.</span><span class="sxs-lookup"><span data-stu-id="ea17a-106">Currently only the directory provider is supported.</span></span> <span data-ttu-id="ea17a-107">Для получения дополнительных сведений см. [разрешения роли администратора в Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span><span class="sxs-lookup"><span data-stu-id="ea17a-107">For more information see [Administrator role permissions in Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>

## <a name="methods"></a><span data-ttu-id="ea17a-108">Методы</span><span class="sxs-lookup"><span data-stu-id="ea17a-108">Methods</span></span>

<span data-ttu-id="ea17a-109">Нет</span><span class="sxs-lookup"><span data-stu-id="ea17a-109">None</span></span>

## <a name="properties"></a><span data-ttu-id="ea17a-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="ea17a-110">Properties</span></span>

<span data-ttu-id="ea17a-111">Нет</span><span class="sxs-lookup"><span data-stu-id="ea17a-111">None</span></span>

## <a name="relationships"></a><span data-ttu-id="ea17a-112">Отношения</span><span class="sxs-lookup"><span data-stu-id="ea17a-112">Relationships</span></span>

| <span data-ttu-id="ea17a-113">Отношение</span><span class="sxs-lookup"><span data-stu-id="ea17a-113">Relationship</span></span> | <span data-ttu-id="ea17a-114">Тип</span><span class="sxs-lookup"><span data-stu-id="ea17a-114">Type</span></span>        | <span data-ttu-id="ea17a-115">Описание</span><span class="sxs-lookup"><span data-stu-id="ea17a-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ea17a-116">каталога</span><span class="sxs-lookup"><span data-stu-id="ea17a-116">directory</span></span>|[<span data-ttu-id="ea17a-117">рбакаппликатион</span><span class="sxs-lookup"><span data-stu-id="ea17a-117">rbacApplication</span></span>](rbacapplication.md)| <span data-ttu-id="ea17a-p102">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="ea17a-p102">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ea17a-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ea17a-120">JSON representation</span></span>

<span data-ttu-id="ea17a-121">Нет</span><span class="sxs-lookup"><span data-stu-id="ea17a-121">None</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "roleManagement resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
