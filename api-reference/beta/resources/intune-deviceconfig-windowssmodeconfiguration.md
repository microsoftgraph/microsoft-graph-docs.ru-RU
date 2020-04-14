---
title: тип перечисления Виндовссмодеконфигуратион
description: Возможные варианты настройки S режима разблокировки
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7dc2eb81f426ca5e8e708fa5b5cdc6904ed9cfa3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43444021"
---
# <a name="windowssmodeconfiguration-enum-type"></a><span data-ttu-id="46f85-103">тип перечисления Виндовссмодеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="46f85-103">windowsSModeConfiguration enum type</span></span>

<span data-ttu-id="46f85-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46f85-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="46f85-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46f85-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46f85-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="46f85-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46f85-107">Возможные варианты настройки S режима разблокировки</span><span class="sxs-lookup"><span data-stu-id="46f85-107">The possible options to configure S mode unlock</span></span>

## <a name="members"></a><span data-ttu-id="46f85-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="46f85-108">Members</span></span>
|<span data-ttu-id="46f85-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="46f85-109">Member</span></span>|<span data-ttu-id="46f85-110">Значение</span><span class="sxs-lookup"><span data-stu-id="46f85-110">Value</span></span>|<span data-ttu-id="46f85-111">Описание</span><span class="sxs-lookup"><span data-stu-id="46f85-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46f85-112">Ограничение</span><span class="sxs-lookup"><span data-stu-id="46f85-112">noRestriction</span></span>|<span data-ttu-id="46f85-113">нуль</span><span class="sxs-lookup"><span data-stu-id="46f85-113">0</span></span>|<span data-ttu-id="46f85-114">Этот параметр удалит все ограничения для режима разблокировки S — значение по умолчанию</span><span class="sxs-lookup"><span data-stu-id="46f85-114">This option will remove all restrictions to unlock S mode - default</span></span>|
|<span data-ttu-id="46f85-115">блок</span><span class="sxs-lookup"><span data-stu-id="46f85-115">block</span></span>|<span data-ttu-id="46f85-116">1,1</span><span class="sxs-lookup"><span data-stu-id="46f85-116">1</span></span>|<span data-ttu-id="46f85-117">Этот параметр блокирует возможность пользователя разблокировать устройство в режиме S</span><span class="sxs-lookup"><span data-stu-id="46f85-117">This option will block the user to unlock the device from S mode</span></span>|
|<span data-ttu-id="46f85-118">блокиру</span><span class="sxs-lookup"><span data-stu-id="46f85-118">unlock</span></span>|<span data-ttu-id="46f85-119">2</span><span class="sxs-lookup"><span data-stu-id="46f85-119">2</span></span>|<span data-ttu-id="46f85-120">Этот параметр позволяет разблокировать устройство в режиме S</span><span class="sxs-lookup"><span data-stu-id="46f85-120">This option will unlock the device from S mode</span></span>|



