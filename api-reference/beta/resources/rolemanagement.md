---
title: Тип ресурса Ролеманажемент
description: Ресурс управления ролями RBAC
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0af20398852e92c69b253dc457c06a954b5e9761
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870126"
---
# <a name="rolemanagement-resource-type"></a><span data-ttu-id="942fa-103">Тип ресурса Ролеманажемент</span><span class="sxs-lookup"><span data-stu-id="942fa-103">roleManagement resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="942fa-104">Объект управления ролями Microsoft 365 RBAC.</span><span class="sxs-lookup"><span data-stu-id="942fa-104">Microsoft 365 RBAC role management entity.</span></span> <span data-ttu-id="942fa-105">Предоставляет доступ к определениям ролей и назначениям ролей, предоставляемым поставщикам RBAC.</span><span class="sxs-lookup"><span data-stu-id="942fa-105">Provides access to role definitions and role assignments surfaced from RBAC providers.</span></span> <span data-ttu-id="942fa-106">В настоящее время поддерживается только поставщик каталогов.</span><span class="sxs-lookup"><span data-stu-id="942fa-106">Currently only the directory provider is supported.</span></span> <span data-ttu-id="942fa-107">Для получения дополнительных сведений см. [разрешения роли администратора в Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span><span class="sxs-lookup"><span data-stu-id="942fa-107">For more information see [Administrator role permissions in Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>

## <a name="methods"></a><span data-ttu-id="942fa-108">Methods</span><span class="sxs-lookup"><span data-stu-id="942fa-108">Methods</span></span>

<span data-ttu-id="942fa-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="942fa-109">None</span></span>

## <a name="properties"></a><span data-ttu-id="942fa-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="942fa-110">Properties</span></span>

<span data-ttu-id="942fa-111">Нет</span><span class="sxs-lookup"><span data-stu-id="942fa-111">None</span></span>

## <a name="relationships"></a><span data-ttu-id="942fa-112">Отношения</span><span class="sxs-lookup"><span data-stu-id="942fa-112">Relationships</span></span>

| <span data-ttu-id="942fa-113">Связь</span><span class="sxs-lookup"><span data-stu-id="942fa-113">Relationship</span></span> | <span data-ttu-id="942fa-114">Тип</span><span class="sxs-lookup"><span data-stu-id="942fa-114">Type</span></span>        | <span data-ttu-id="942fa-115">Описание</span><span class="sxs-lookup"><span data-stu-id="942fa-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="942fa-116">каталога</span><span class="sxs-lookup"><span data-stu-id="942fa-116">directory</span></span>|[<span data-ttu-id="942fa-117">рбакаппликатион</span><span class="sxs-lookup"><span data-stu-id="942fa-117">rbacApplication</span></span>](rbacapplication.md)| <span data-ttu-id="942fa-p102">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="942fa-p102">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="942fa-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="942fa-120">JSON representation</span></span>

<span data-ttu-id="942fa-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="942fa-121">None</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "roleManagement resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
