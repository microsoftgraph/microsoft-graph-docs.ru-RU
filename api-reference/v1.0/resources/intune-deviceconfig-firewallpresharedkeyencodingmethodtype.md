---
title: тип перечисления Фиреваллпрешаредкэйенкодингмесодтипе
description: Возможные значения для Фиреваллпрешаредкэйенкодингмесод
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: dadb35cb95db83c03c74bdb2e4eac70a5951cc5e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532521"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="38803-103">тип перечисления Фиреваллпрешаредкэйенкодингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="38803-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

<span data-ttu-id="38803-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38803-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="38803-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="38803-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38803-106">Возможные значения для Фиреваллпрешаредкэйенкодингмесод</span><span class="sxs-lookup"><span data-stu-id="38803-106">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="38803-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="38803-107">Members</span></span>
|<span data-ttu-id="38803-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="38803-108">Member</span></span>|<span data-ttu-id="38803-109">Значение</span><span class="sxs-lookup"><span data-stu-id="38803-109">Value</span></span>|<span data-ttu-id="38803-110">Описание</span><span class="sxs-lookup"><span data-stu-id="38803-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38803-111">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="38803-111">deviceDefault</span></span>|<span data-ttu-id="38803-112">нуль</span><span class="sxs-lookup"><span data-stu-id="38803-112">0</span></span>|<span data-ttu-id="38803-113">Значение не настроено Intune, не переопределять значение устройства по умолчанию, настроенное пользователем</span><span class="sxs-lookup"><span data-stu-id="38803-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="38803-114">нет</span><span class="sxs-lookup"><span data-stu-id="38803-114">none</span></span>|<span data-ttu-id="38803-115">1 </span><span class="sxs-lookup"><span data-stu-id="38803-115">1</span></span>|<span data-ttu-id="38803-116">Общий ключ не кодируется.</span><span class="sxs-lookup"><span data-stu-id="38803-116">Preshared key is not encoded.</span></span> <span data-ttu-id="38803-117">Вместо этого он хранится в расширенном формате символов</span><span class="sxs-lookup"><span data-stu-id="38803-117">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="38803-118">utF8</span><span class="sxs-lookup"><span data-stu-id="38803-118">utF8</span></span>|<span data-ttu-id="38803-119">2 </span><span class="sxs-lookup"><span data-stu-id="38803-119">2</span></span>|<span data-ttu-id="38803-120">Кодирование общего ключа с помощью UTF – 8</span><span class="sxs-lookup"><span data-stu-id="38803-120">Encode the preshared key using UTF-8</span></span>|




