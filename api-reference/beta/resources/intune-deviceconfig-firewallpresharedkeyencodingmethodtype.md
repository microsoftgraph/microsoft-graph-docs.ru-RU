---
title: тип перечисления Фиреваллпрешаредкэйенкодингмесодтипе
description: Возможные значения для Фиреваллпрешаредкэйенкодингмесод
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ddd167d69674c0e32c184aa0f68bd7698331ee3c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36004306"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="c5c5e-103">тип перечисления Фиреваллпрешаредкэйенкодингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="c5c5e-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="c5c5e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5c5e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5c5e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c5c5e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5c5e-106">Возможные значения для Фиреваллпрешаредкэйенкодингмесод</span><span class="sxs-lookup"><span data-stu-id="c5c5e-106">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="c5c5e-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="c5c5e-107">Members</span></span>
|<span data-ttu-id="c5c5e-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="c5c5e-108">Member</span></span>|<span data-ttu-id="c5c5e-109">Значение</span><span class="sxs-lookup"><span data-stu-id="c5c5e-109">Value</span></span>|<span data-ttu-id="c5c5e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c5c5e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5c5e-111">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="c5c5e-111">deviceDefault</span></span>|<span data-ttu-id="c5c5e-112">нуль</span><span class="sxs-lookup"><span data-stu-id="c5c5e-112">0</span></span>|<span data-ttu-id="c5c5e-113">Значение не настроено Intune, не переопределять значение устройства по умолчанию, настроенное пользователем</span><span class="sxs-lookup"><span data-stu-id="c5c5e-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="c5c5e-114">none</span><span class="sxs-lookup"><span data-stu-id="c5c5e-114">none</span></span>|<span data-ttu-id="c5c5e-115">1,1</span><span class="sxs-lookup"><span data-stu-id="c5c5e-115">1</span></span>|<span data-ttu-id="c5c5e-116">Общий ключ не кодируется.</span><span class="sxs-lookup"><span data-stu-id="c5c5e-116">Preshared key is not encoded.</span></span> <span data-ttu-id="c5c5e-117">Вместо этого он хранится в расширенном формате символов</span><span class="sxs-lookup"><span data-stu-id="c5c5e-117">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="c5c5e-118">utF8</span><span class="sxs-lookup"><span data-stu-id="c5c5e-118">utF8</span></span>|<span data-ttu-id="c5c5e-119">2</span><span class="sxs-lookup"><span data-stu-id="c5c5e-119">2</span></span>|<span data-ttu-id="c5c5e-120">Кодирование общего ключа с помощью UTF – 8</span><span class="sxs-lookup"><span data-stu-id="c5c5e-120">Encode the preshared key using UTF-8</span></span>|





