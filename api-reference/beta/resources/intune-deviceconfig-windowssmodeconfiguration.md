---
title: тип перечисления Виндовссмодеконфигуратион
description: Возможные варианты настройки S режима разблокировки
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: bd9b4c696c7456e4cf926764bfadde3fbd591a6e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525406"
---
# <a name="windowssmodeconfiguration-enum-type"></a><span data-ttu-id="060c5-103">тип перечисления Виндовссмодеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="060c5-103">windowsSModeConfiguration enum type</span></span>

<span data-ttu-id="060c5-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="060c5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="060c5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="060c5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="060c5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="060c5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="060c5-107">Возможные варианты настройки S режима разблокировки</span><span class="sxs-lookup"><span data-stu-id="060c5-107">The possible options to configure S mode unlock</span></span>

## <a name="members"></a><span data-ttu-id="060c5-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="060c5-108">Members</span></span>
|<span data-ttu-id="060c5-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="060c5-109">Member</span></span>|<span data-ttu-id="060c5-110">Значение</span><span class="sxs-lookup"><span data-stu-id="060c5-110">Value</span></span>|<span data-ttu-id="060c5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="060c5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="060c5-112">Ограничение</span><span class="sxs-lookup"><span data-stu-id="060c5-112">noRestriction</span></span>|<span data-ttu-id="060c5-113">нуль</span><span class="sxs-lookup"><span data-stu-id="060c5-113">0</span></span>|<span data-ttu-id="060c5-114">Этот параметр удалит все ограничения для режима разблокировки S — значение по умолчанию</span><span class="sxs-lookup"><span data-stu-id="060c5-114">This option will remove all restrictions to unlock S mode - default</span></span>|
|<span data-ttu-id="060c5-115">блок</span><span class="sxs-lookup"><span data-stu-id="060c5-115">block</span></span>|<span data-ttu-id="060c5-116">1 </span><span class="sxs-lookup"><span data-stu-id="060c5-116">1</span></span>|<span data-ttu-id="060c5-117">Этот параметр блокирует возможность пользователя разблокировать устройство в режиме S</span><span class="sxs-lookup"><span data-stu-id="060c5-117">This option will block the user to unlock the device from S mode</span></span>|
|<span data-ttu-id="060c5-118">блокиру</span><span class="sxs-lookup"><span data-stu-id="060c5-118">unlock</span></span>|<span data-ttu-id="060c5-119">2 </span><span class="sxs-lookup"><span data-stu-id="060c5-119">2</span></span>|<span data-ttu-id="060c5-120">Этот параметр позволяет разблокировать устройство в режиме S</span><span class="sxs-lookup"><span data-stu-id="060c5-120">This option will unlock the device from S mode</span></span>|



