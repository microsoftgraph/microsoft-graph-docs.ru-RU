---
title: встроенный тип enumSIMDeviceStateValue
description: Описывает различные состояния встроенного кода активации SIM-карты.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ab8db5b259c78ed48a3f1de4a0732dfeb69212d6
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58785726"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a>встроенный тип enumSIMDeviceStateValue

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Описывает различные состояния встроенного кода активации SIM-карты.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|notEvaluated|0|Обозначает, что встроенный код активации SIM-карты является бесплатным и доступным для присвоения устройству.|
|не удалось|1|Обозначает, что службе Intune не удалось доставить этот профиль на устройство.|
|установка|2|Обозначает, что встроенный код активации SIM-карты назначен устройству и устройство устанавливает маркер.|
|установлено|3|Обозначает успешное установку встроенного кода активации SIM-карты на целевом устройстве.|
|удаление|4 |Обозначает, что служба Intune пытается удалить профиль с устройства.|
|error|5 |Обозначает ошибку с этим профилем.|
|deleted|6 |Обозначает, что профиль удаляется с устройства.|
|removedByUser|7 |Обозначает, что профиль удаляется с устройства пользователем|



