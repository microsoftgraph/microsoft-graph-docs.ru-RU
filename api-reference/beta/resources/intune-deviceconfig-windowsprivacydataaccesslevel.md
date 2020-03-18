---
title: тип перечисления Виндовспривацидатаакцесслевел
description: Определите категорию уровня доступа к определенной конфиденциальной информации Windows.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 96ef43bae6996c3268a3e0d268f80267e192deee
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42786252"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a><span data-ttu-id="cd6db-103">тип перечисления Виндовспривацидатаакцесслевел</span><span class="sxs-lookup"><span data-stu-id="cd6db-103">windowsPrivacyDataAccessLevel enum type</span></span>

> <span data-ttu-id="cd6db-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd6db-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cd6db-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cd6db-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd6db-106">Определите категорию уровня доступа к определенной конфиденциальной информации Windows.</span><span class="sxs-lookup"><span data-stu-id="cd6db-106">Determine the access level to specific Windows privacy data category.</span></span>

## <a name="members"></a><span data-ttu-id="cd6db-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="cd6db-107">Members</span></span>
|<span data-ttu-id="cd6db-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="cd6db-108">Member</span></span>|<span data-ttu-id="cd6db-109">Значение</span><span class="sxs-lookup"><span data-stu-id="cd6db-109">Value</span></span>|<span data-ttu-id="cd6db-110">Описание</span><span class="sxs-lookup"><span data-stu-id="cd6db-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd6db-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="cd6db-111">notConfigured</span></span>|<span data-ttu-id="cd6db-112">нуль</span><span class="sxs-lookup"><span data-stu-id="cd6db-112">0</span></span>|<span data-ttu-id="cd6db-113">Уровень доступа не указан, нет целей.</span><span class="sxs-lookup"><span data-stu-id="cd6db-113">No access level specified, no intents.</span></span> <span data-ttu-id="cd6db-114">Устройство может вести себя как в Усеринконтрол, так и Форцеаллов.</span><span class="sxs-lookup"><span data-stu-id="cd6db-114">Device may behave either as in UserInControl or ForceAllow.</span></span> <span data-ttu-id="cd6db-115">Это может зависеть от данных о конфиденциальности, а также версий Windows и других факторов.</span><span class="sxs-lookup"><span data-stu-id="cd6db-115">It may depend on the privacy data been accessed, Windows versions and other factors.</span></span>|
|<span data-ttu-id="cd6db-116">форцеаллов</span><span class="sxs-lookup"><span data-stu-id="cd6db-116">forceAllow</span></span>|<span data-ttu-id="cd6db-117">1,1</span><span class="sxs-lookup"><span data-stu-id="cd6db-117">1</span></span>|<span data-ttu-id="cd6db-118">Приложениям будет разрешен доступ к указанным данным о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="cd6db-118">Apps will be allowed to access the specified privacy data.</span></span>|
|<span data-ttu-id="cd6db-119">форцедени</span><span class="sxs-lookup"><span data-stu-id="cd6db-119">forceDeny</span></span>|<span data-ttu-id="cd6db-120">2</span><span class="sxs-lookup"><span data-stu-id="cd6db-120">2</span></span>|<span data-ttu-id="cd6db-121">Приложениям будет отказано в доступе к указанным данным о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="cd6db-121">Apps will be denied to access specified privacy data.</span></span>|
|<span data-ttu-id="cd6db-122">усеринконтрол</span><span class="sxs-lookup"><span data-stu-id="cd6db-122">userInControl</span></span>|<span data-ttu-id="cd6db-123">4</span><span class="sxs-lookup"><span data-stu-id="cd6db-123">3</span></span>|<span data-ttu-id="cd6db-124">Пользователи будут получать приглашение при попытке приложения получить доступ к указанным данным о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="cd6db-124">Users will be prompted when apps try to access specified privacy data.</span></span>|



