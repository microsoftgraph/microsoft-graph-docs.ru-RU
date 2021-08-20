---
title: тип переуправления managementState
description: Состояние управления устройством в Microsoft Intune.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1475ac4dc29462b31df57ae54daf4ecb658487133ad5b0fe2cc5884e8effdc5a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54249876"
---
# <a name="managementstate-enum-type"></a>тип переуправления managementState

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние управления устройством в Microsoft Intune.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|управляемый|0|Устройство находится под управлением|
|retirePending|1 |На устройстве и в процессе отгрузки из управления возникает команда по отставку|
|retireFailed|2|На устройстве сбой команды по отставку|
|wipePending|3 |Команда wipe происходит на устройстве и в процессе отгрузки из управления|
|wipeFailed|4 |Команда Wipe сбой на устройстве|
|нездоровый|5 |Устройство является нездоровым.|
|deletePending|6 |На устройстве возникает команда удаления |
|retireIssued|7 |Для устройства была выдана команда на отставку|
|wipeIssued|8 |Для устройства была выдана команда wipe|
|wipeCanceled|9 |Команда wipe для этого устройства отменена|
|retireCanceled|10 |Команда отмены для этого устройства отменена|
|обнаружено|11 |Устройство обнаружено, но не полностью зарегистрировано.|




