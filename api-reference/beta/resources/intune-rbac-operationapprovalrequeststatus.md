---
title: Тип перечисления operationApprovalRequestStatus
description: Состояние текущего запроса на утверждение
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0068b5805ec8668e75a470b6d94ca16cdab2ca0e
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65210740"
---
# <a name="operationapprovalrequeststatus-enum-type"></a>Тип перечисления operationApprovalRequestStatus

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние текущего запроса на утверждение

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Неизвестное состояние|
|needsApproval|1|Перед выполнением действия запрос на утверждение должен быть одобрен.|
|Утвержденных|2|Запрос на утверждение утвержден, теперь можно выполнить действие.|
|Отклонено|3|Запрос на утверждение отклонен, действие не утверждено и дальнейшие действия не могут быть выполнены.|
|Отменен|4|Запрос на утверждение отменен пользователем, не требуя дальнейших действий.|
|Завершена|5|Запрос на утверждение завершен, никаких дальнейших действий не требуется.|
|Истек|6 |Срок действия запроса на утверждение истек, для выполнения этого запроса необходимо выполнить новое утверждение.|
|unknownFutureValue|99|Заполнитель для будущих состояний запроса на утверждение операции.|




